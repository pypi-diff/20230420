# Comparing `tmp/odroid_wiringpi-3.7.tar.gz` & `tmp/odroid_wiringpi-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odroid_wiringpi-3.7.tar", last modified: Tue Sep  8 01:27:45 2020, max compression
+gzip compressed data, was "dist/odroid_wiringpi-3.8.tar", last modified: Thu Nov 19 03:05:29 2020, max compression
```

## Comparing `odroid_wiringpi-3.7.tar` & `odroid_wiringpi-3.8.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-09-08 01:27:45.000711 odroid_wiringpi-3.7/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7651 2020-08-18 05:45:56.000000 odroid_wiringpi-3.7/LICENSE.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      179 2020-08-18 05:45:56.000000 odroid_wiringpi-3.7/MANIFEST.in
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5381 2020-09-08 01:27:45.004711 odroid_wiringpi-3.7/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3922 2020-08-18 05:45:56.000000 odroid_wiringpi-3.7/README.rst
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-09-08 01:27:44.992711 odroid_wiringpi-3.7/WiringPi/
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-09-08 01:27:44.992711 odroid_wiringpi-3.7/WiringPi/devLib/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5866 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/ds1302.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1673 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/ds1302.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    55558 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/font.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4119 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/gertboard.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1484 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/gertboard.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    11549 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/lcd.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2095 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/lcd.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    14788 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/lcd128x64.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2077 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/lcd128x64.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5658 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/maxdetect.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1266 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/maxdetect.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3286 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/piFace.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1161 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/piFace.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2981 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/piGlow.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1486 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/piGlow.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2915 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/piNes.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1446 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/piNes.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     9364 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/scrollPhat.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1778 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/scrollPhat.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7253 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/devLib/scrollPhatFont.h
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-09-08 01:27:44.992711 odroid_wiringpi-3.7/WiringPi/examples/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1011 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/examples/header.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       72 2020-09-08 01:25:53.000000 odroid_wiringpi-3.7/WiringPi/version.h
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-09-08 01:27:45.000711 odroid_wiringpi-3.7/WiringPi/wiringPi/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     8907 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/ads1115.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1604 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/ads1115.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     6148 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/bmp180.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1176 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/bmp180.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    10071 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/drcNet.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1364 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/drcNet.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5122 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/drcSerial.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1228 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/drcSerial.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3519 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/ds18b20.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1200 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/ds18b20.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3531 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/htu21d.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1176 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/htu21d.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2811 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/max31855.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1181 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/max31855.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2374 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/max5322.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/max5322.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3727 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23008.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1185 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23008.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3854 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23016.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1188 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23016.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1545 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23016reg.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4400 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23017.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1185 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23017.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4654 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s08.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1199 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s08.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5420 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s17.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1181 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s17.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2026 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23x08.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2588 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23x0817.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2167 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3002.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3002.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2224 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3004.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3004.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3547 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3422.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1355 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3422.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2198 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp4802.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/mcp4802.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      662 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroid_template.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    22433 2020-08-24 08:58:13.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc1.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1832 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc1.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    24822 2020-08-24 08:58:13.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc2.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2023 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc2.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    20563 2020-09-08 01:25:53.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc4.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2236 2020-09-08 01:25:53.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc4.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    22381 2020-08-24 08:58:13.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn1.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2150 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn1.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    26185 2020-08-24 08:58:13.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn2.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2557 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn2.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    21669 2020-08-24 08:58:13.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidxu3.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2105 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/odroidxu3.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3252 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8574.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1184 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8574.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2677 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8591.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1191 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8591.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1619 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/piHiPri.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1806 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/piThread.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2803 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/pseudoPins.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1143 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/pseudoPins.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5926 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/rht03.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1115 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/rht03.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2389 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/sn3218.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1157 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/sn3218.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4727 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/softPwm.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1250 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/softPwm.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     6350 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/softServo.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1283 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/softServo.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3539 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/softTone.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1428 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/softTone.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3216 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/sr595.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1230 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/sr595.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    34781 2020-09-08 01:25:53.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPi.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    10782 2020-08-25 08:57:07.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPi.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7148 2020-09-08 01:25:53.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiI2C.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1704 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiI2C.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4923 2020-08-24 08:58:13.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiSPI.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1404 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiSPI.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     6007 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringSerial.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1496 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringSerial.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2283 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringShift.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1367 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wiringShift.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    20261 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wpiExtensions.c
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1189 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPi/wpiExtensions.h
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-09-08 01:27:45.000711 odroid_wiringpi-3.7/WiringPi/wiringPiD/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      266 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPiD/daemonise.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1366 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPiD/drcNetCmd.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1363 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPiD/network.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     1129 2020-08-24 08:56:16.000000 odroid_wiringpi-3.7/WiringPi/wiringPiD/runRemote.h
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    11940 2020-08-24 05:56:41.000000 odroid_wiringpi-3.7/bindings.i
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      584 2020-08-18 05:45:56.000000 odroid_wiringpi-3.7/constants.py
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-09-08 01:27:45.000711 odroid_wiringpi-3.7/odroid_wiringpi.egg-info/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     5381 2020-09-08 01:27:44.000000 odroid_wiringpi-3.7/odroid_wiringpi.egg-info/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3376 2020-09-08 01:27:44.000000 odroid_wiringpi-3.7/odroid_wiringpi.egg-info/SOURCES.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2020-09-08 01:27:44.000000 odroid_wiringpi-3.7/odroid_wiringpi.egg-info/dependency_links.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       33 2020-09-08 01:27:44.000000 odroid_wiringpi-3.7/odroid_wiringpi.egg-info/top_level.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    22279 2020-09-08 01:27:39.000000 odroid_wiringpi-3.7/odroid_wiringpi.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      303 2020-09-08 01:27:45.004711 odroid_wiringpi-3.7/setup.cfg
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     2146 2020-09-08 01:26:08.000000 odroid_wiringpi-3.7/setup.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     4851 2020-08-18 05:45:56.000000 odroid_wiringpi-3.7/wiringpi-class.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)    12957 2020-08-18 05:45:56.000000 odroid_wiringpi-3.7/wiringpi.i
--rw-rw-r--   0 joshua    (1000) joshua    (1000)   305147 2020-09-08 01:27:39.000000 odroid_wiringpi-3.7/wiringpi_wrap.c
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-11-19 03:05:29.029727 odroid_wiringpi-3.8/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7651 2020-06-26 06:25:31.000000 odroid_wiringpi-3.8/LICENSE.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      179 2020-06-26 06:25:31.000000 odroid_wiringpi-3.8/MANIFEST.in
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5381 2020-11-19 03:05:29.029727 odroid_wiringpi-3.8/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3922 2020-06-26 06:25:31.000000 odroid_wiringpi-3.8/README.rst
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-11-19 03:05:28.997724 odroid_wiringpi-3.8/WiringPi/
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-11-19 03:05:29.005725 odroid_wiringpi-3.8/WiringPi/devLib/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5866 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/ds1302.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1673 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/ds1302.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    55558 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/font.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4119 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/gertboard.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1484 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/gertboard.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    11549 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/lcd.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2095 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/lcd.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    14788 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/lcd128x64.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2077 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/lcd128x64.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5658 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/maxdetect.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1266 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/maxdetect.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3286 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/piFace.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1161 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/piFace.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2981 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/piGlow.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1486 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/piGlow.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2915 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/piNes.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1446 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/piNes.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     9364 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/scrollPhat.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1778 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/scrollPhat.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7253 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/devLib/scrollPhatFont.h
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-11-19 03:05:29.005725 odroid_wiringpi-3.8/WiringPi/examples/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1011 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/examples/header.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       72 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/version.h
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-11-19 03:05:29.025727 odroid_wiringpi-3.8/WiringPi/wiringPi/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     8907 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/ads1115.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1604 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/ads1115.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     6148 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/bmp180.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1176 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/bmp180.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    10071 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/drcNet.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1364 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/drcNet.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5122 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/drcSerial.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1228 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/drcSerial.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3519 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/ds18b20.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1200 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/ds18b20.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3531 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/htu21d.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1176 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/htu21d.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2811 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/max31855.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1181 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/max31855.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2374 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/max5322.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/max5322.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3727 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23008.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1185 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23008.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3854 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23016.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1188 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23016.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1545 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23016reg.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4400 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23017.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1185 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23017.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4654 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s08.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1199 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s08.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5420 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s17.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1181 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s17.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2026 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23x08.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2588 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23x0817.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2167 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3002.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3002.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2224 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3004.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3004.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3547 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3422.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1355 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3422.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2198 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp4802.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1186 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/mcp4802.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      662 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroid_template.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    22433 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc1.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1832 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc1.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    24822 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc2.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2023 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc2.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    20563 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc4.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2294 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc4.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    16528 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidhc4.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    22381 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn1.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2150 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn1.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    26185 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn2.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2557 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn2.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    21669 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidxu3.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2105 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/odroidxu3.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3252 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8574.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1184 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8574.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2677 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8591.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1191 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8591.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1619 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/piHiPri.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1806 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/piThread.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2803 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/pseudoPins.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1143 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/pseudoPins.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5926 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/rht03.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1115 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/rht03.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2389 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/sn3218.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1157 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/sn3218.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4727 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/softPwm.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1250 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/softPwm.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     6350 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/softServo.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1283 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/softServo.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3539 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/softTone.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1428 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/softTone.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3216 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/sr595.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1230 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/sr595.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    34973 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPi.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    10809 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPi.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7172 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiI2C.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1704 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiI2C.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5022 2020-11-19 03:04:41.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiSPI.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1404 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiSPI.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     6007 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringSerial.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1496 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringSerial.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2283 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringShift.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1367 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wiringShift.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    20261 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wpiExtensions.c
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1189 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPi/wpiExtensions.h
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-11-19 03:05:29.029727 odroid_wiringpi-3.8/WiringPi/wiringPiD/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      266 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPiD/daemonise.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1366 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPiD/drcNetCmd.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1363 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPiD/network.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1129 2020-06-26 06:26:13.000000 odroid_wiringpi-3.8/WiringPi/wiringPiD/runRemote.h
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    11940 2020-11-19 03:04:07.000000 odroid_wiringpi-3.8/bindings.i
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      584 2020-06-26 06:25:31.000000 odroid_wiringpi-3.8/constants.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2020-11-19 03:05:29.029727 odroid_wiringpi-3.8/odroid_wiringpi.egg-info/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     5381 2020-11-19 03:05:28.000000 odroid_wiringpi-3.8/odroid_wiringpi.egg-info/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3406 2020-11-19 03:05:28.000000 odroid_wiringpi-3.8/odroid_wiringpi.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2020-11-19 03:05:28.000000 odroid_wiringpi-3.8/odroid_wiringpi.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       33 2020-11-19 03:05:28.000000 odroid_wiringpi-3.8/odroid_wiringpi.egg-info/top_level.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    22279 2020-11-19 03:05:14.000000 odroid_wiringpi-3.8/odroid_wiringpi.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      303 2020-11-19 03:05:29.029727 odroid_wiringpi-3.8/setup.cfg
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     2146 2020-11-19 03:04:54.000000 odroid_wiringpi-3.8/setup.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4851 2020-06-26 06:25:31.000000 odroid_wiringpi-3.8/wiringpi-class.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)    12957 2020-06-26 06:25:31.000000 odroid_wiringpi-3.8/wiringpi.i
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)   305147 2020-11-19 03:05:14.000000 odroid_wiringpi-3.8/wiringpi_wrap.c
```

### Comparing `odroid_wiringpi-3.7/LICENSE.txt` & `odroid_wiringpi-3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/PKG-INFO` & `odroid_wiringpi-3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: odroid_wiringpi
-Version: 3.7
+Version: 3.8
 Summary: A Port of WiringPi Python project for ODROID boards
 Home-page: https://github.com/hardkernel/WiringPi2-Python
 Author: Deokgyu Yang
 Author-email: secugyu@gmail.com
 License: LGPL
 Description: Note
         ~~~~
```

### Comparing `odroid_wiringpi-3.7/README.rst` & `odroid_wiringpi-3.8/README.rst`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/ds1302.c` & `odroid_wiringpi-3.8/WiringPi/devLib/ds1302.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/ds1302.h` & `odroid_wiringpi-3.8/WiringPi/devLib/ds1302.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/font.h` & `odroid_wiringpi-3.8/WiringPi/devLib/font.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/gertboard.c` & `odroid_wiringpi-3.8/WiringPi/devLib/gertboard.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/gertboard.h` & `odroid_wiringpi-3.8/WiringPi/devLib/gertboard.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/lcd.c` & `odroid_wiringpi-3.8/WiringPi/devLib/lcd.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/lcd.h` & `odroid_wiringpi-3.8/WiringPi/devLib/lcd.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/lcd128x64.c` & `odroid_wiringpi-3.8/WiringPi/devLib/lcd128x64.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/lcd128x64.h` & `odroid_wiringpi-3.8/WiringPi/devLib/lcd128x64.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/maxdetect.c` & `odroid_wiringpi-3.8/WiringPi/devLib/maxdetect.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/maxdetect.h` & `odroid_wiringpi-3.8/WiringPi/devLib/maxdetect.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/piFace.c` & `odroid_wiringpi-3.8/WiringPi/devLib/piFace.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/piFace.h` & `odroid_wiringpi-3.8/WiringPi/devLib/piFace.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/piGlow.c` & `odroid_wiringpi-3.8/WiringPi/devLib/piGlow.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/piGlow.h` & `odroid_wiringpi-3.8/WiringPi/devLib/piGlow.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/piNes.c` & `odroid_wiringpi-3.8/WiringPi/devLib/piNes.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/piNes.h` & `odroid_wiringpi-3.8/WiringPi/devLib/piNes.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/scrollPhat.c` & `odroid_wiringpi-3.8/WiringPi/devLib/scrollPhat.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/scrollPhat.h` & `odroid_wiringpi-3.8/WiringPi/devLib/scrollPhat.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/devLib/scrollPhatFont.h` & `odroid_wiringpi-3.8/WiringPi/devLib/scrollPhatFont.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/examples/header.h` & `odroid_wiringpi-3.8/WiringPi/examples/header.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/ads1115.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/ads1115.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/ads1115.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/ads1115.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/bmp180.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/bmp180.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/bmp180.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/bmp180.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/drcNet.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/drcNet.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/drcNet.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/drcNet.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/drcSerial.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/drcSerial.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/drcSerial.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/drcSerial.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/ds18b20.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/ds18b20.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/ds18b20.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/ds18b20.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/htu21d.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/htu21d.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/htu21d.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/htu21d.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/max31855.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/max31855.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/max31855.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/max31855.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/max5322.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/max5322.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/max5322.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/max5322.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23008.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23008.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23008.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23008.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23016.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23016.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23016.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23016.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23016reg.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23016reg.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23017.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23017.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23017.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23017.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s08.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s08.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s08.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s08.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s17.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s17.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23s17.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23s17.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23x08.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23x08.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp23x0817.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp23x0817.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3002.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3002.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3002.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3002.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3004.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3004.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3004.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3004.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3422.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3422.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp3422.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp3422.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp4802.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp4802.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/mcp4802.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/mcp4802.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroid_template.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroid_template.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc1.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc1.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc1.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc1.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc2.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc2.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc2.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc2.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc4.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc4.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidc4.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidc4.h`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 #define C4_GPIOX_MUX_5_REG_OFFSET	0x1B5
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 extern void init_odroidc4 (struct libodroid *libwiring);
+extern void init_odroidhc4 (struct libodroid *libwiring);
 
 #ifdef __cplusplus
 }
 #endif
 
 /*----------------------------------------------------------------------------*/
 #endif	/* __ODROID_C4_H__ */
```

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn1.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn1.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn1.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn1.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn2.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn2.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidn2.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidn2.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidxu3.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidxu3.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/odroidxu3.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/odroidxu3.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8574.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8574.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8574.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8574.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8591.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8591.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/pcf8591.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/pcf8591.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/piHiPri.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/piHiPri.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/piThread.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/piThread.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/pseudoPins.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/pseudoPins.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/pseudoPins.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/pseudoPins.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/rht03.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/rht03.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/rht03.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/rht03.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/sn3218.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/sn3218.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/sn3218.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/sn3218.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/softPwm.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/softPwm.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/softPwm.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/softPwm.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/softServo.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/softServo.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/softServo.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/softServo.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/softTone.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/softTone.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/softTone.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/softTone.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/sr595.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/sr595.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/sr595.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/sr595.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPi.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPi.c`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 	"Unknown",
 	"ODROID-C1/C1+",
 	"ODROID-C2",
 	"ODROID-XU3/XU4",
 	"ODROID-N1",
 	"ODROID-N2/N2Plus",
 	"ODROID-C4",
+	"ODROID-HC4",
 };
 
 const char *piRevisionNames [16] =
 {
 	"00",
 	"01",
 	"02",
@@ -497,14 +498,19 @@
 			libwiring.rev = 1;
 			break;
 		case MODEL_ODROID_C4:
 			libwiring.maker = MAKER_AMLOGIC;
 			libwiring.mem = 4;
 			libwiring.rev = 1;
 			break;
+		case MODEL_ODROID_HC4:
+			libwiring.maker = MAKER_AMLOGIC;
+			libwiring.mem = 4;
+			libwiring.rev = 1;
+			break;
 		case MODEL_UNKNOWN:
 		default:
 			libwiring.model = MAKER_UNKNOWN;
 			libwiring.maker = MAKER_UNKNOWN;
 			libwiring.mem = 0;
 			libwiring.rev = 0;
 	}
@@ -1204,14 +1210,17 @@
 	break;
 	case MODEL_ODROID_N2:
 		init_odroidn2(&libwiring);
 	break;
 	case MODEL_ODROID_C4:
 		init_odroidc4(&libwiring);
 	break;
+	case MODEL_ODROID_HC4:
+		init_odroidhc4(&libwiring);
+	break;
 	default:
 		return wiringPiFailure (WPI_ALMOST,
 			"wiringPiSetup: Unknown model\n");
 	}
 
 	initialiseEpoch ();
```

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPi.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPi.h`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 #define	MODEL_UNKNOWN		0
 #define	MODEL_ODROID_C1		1
 #define	MODEL_ODROID_C2		2
 #define	MODEL_ODROID_XU3	3
 #define	MODEL_ODROID_N1		4
 #define	MODEL_ODROID_N2		5
 #define	MODEL_ODROID_C4		6
+#define	MODEL_ODROID_HC4	7
 
 #define	MAKER_UNKNOWN		0
 #define	MAKER_AMLOGIC		1
 #define	MAKER_SAMSUNG		2
 #define	MAKER_ROCKCHIP		3
 
 #define	MODE_PINS		0
```

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiI2C.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiI2C.c`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,15 @@
 			device = "/dev/i2c-1";
 	break;
 	case MODEL_ODROID_N1:
 		device = "/dev/i2c-4";
 	break;
 	case MODEL_ODROID_N2:
 	case MODEL_ODROID_C4:
+	case MODEL_ODROID_HC4:
 		if (cmpKernelVersion(KERN_NUM_TO_REVISION, 4, 9, 230))
 			device = "/dev/i2c-0";
 		else
 			device = "/dev/i2c-2";
 	break;
 	}
```

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiI2C.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiI2C.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiSPI.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiSPI.c`

 * *Files 2% similar despite different names*

```diff
@@ -134,20 +134,21 @@
 int wiringPiSPISetupMode (int channel, int speed, int mode)
 {
 	char device[25];
 	int model, temp;
 
 	piBoardId (&model, &temp, &temp, &temp, &temp) ;
 
-	if (model == MODEL_ODROID_C2) {
+	switch(model)	{
+	case MODEL_ODROID_C2:
 		return wiringPiFailure (WPI_ALMOST,
 			"ODROID C2 does not support hardware SPI. Check out the SPI bitbang and use wiringPiSPISetupInterface.\n");
-	}
-
-	switch(model)	{
+	case MODEL_ODROID_HC4:
+		return wiringPiFailure (WPI_ALMOST,
+			"ODROID HC4 does not support hardware SPI.\n");
 	case MODEL_ODROID_C1:
 	case MODEL_ODROID_N2:
 	case MODEL_ODROID_C4:
 		sprintf(device, "%s%d", spiDevType0, channel);
 	break;
 	case MODEL_ODROID_XU3:
 		if (cmpKernelVersion(KERN_NUM_TO_MAJOR, 5))
```

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringPiSPI.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringPiSPI.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringSerial.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringSerial.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringSerial.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringSerial.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringShift.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringShift.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wiringShift.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wiringShift.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wpiExtensions.c` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wpiExtensions.c`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPi/wpiExtensions.h` & `odroid_wiringpi-3.8/WiringPi/wiringPi/wpiExtensions.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPiD/drcNetCmd.h` & `odroid_wiringpi-3.8/WiringPi/wiringPiD/drcNetCmd.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPiD/network.h` & `odroid_wiringpi-3.8/WiringPi/wiringPiD/network.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/WiringPi/wiringPiD/runRemote.h` & `odroid_wiringpi-3.8/WiringPi/wiringPiD/runRemote.h`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/bindings.i` & `odroid_wiringpi-3.8/bindings.i`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/constants.py` & `odroid_wiringpi-3.8/constants.py`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/odroid_wiringpi.egg-info/PKG-INFO` & `odroid_wiringpi-3.8/odroid_wiringpi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: odroid-wiringpi
-Version: 3.7
+Version: 3.8
 Summary: A Port of WiringPi Python project for ODROID boards
 Home-page: https://github.com/hardkernel/WiringPi2-Python
 Author: Deokgyu Yang
 Author-email: secugyu@gmail.com
 License: LGPL
 Description: Note
         ~~~~
```

### Comparing `odroid_wiringpi-3.7/odroid_wiringpi.egg-info/SOURCES.txt` & `odroid_wiringpi-3.8/odroid_wiringpi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 WiringPi/wiringPi/odroid_template.h
 WiringPi/wiringPi/odroidc1.c
 WiringPi/wiringPi/odroidc1.h
 WiringPi/wiringPi/odroidc2.c
 WiringPi/wiringPi/odroidc2.h
 WiringPi/wiringPi/odroidc4.c
 WiringPi/wiringPi/odroidc4.h
+WiringPi/wiringPi/odroidhc4.c
 WiringPi/wiringPi/odroidn1.c
 WiringPi/wiringPi/odroidn1.h
 WiringPi/wiringPi/odroidn2.c
 WiringPi/wiringPi/odroidn2.h
 WiringPi/wiringPi/odroidxu3.c
 WiringPi/wiringPi/odroidxu3.h
 WiringPi/wiringPi/pcf8574.c
```

### Comparing `odroid_wiringpi-3.7/odroid_wiringpi.py` & `odroid_wiringpi-3.8/odroid_wiringpi.py`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/setup.py` & `odroid_wiringpi-3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,13 +60,13 @@
     sources=sources,
     swig_opts=['-threads'],
     extra_link_args=['-lcrypt', '-lrt'],
 )
 
 setup(
     name = 'odroid_wiringpi',
-    version = '3.7',
+    version = '3.8',
     ext_modules = [ _odroid_wiringpi ],
     py_modules = ["odroid_wiringpi"],
     install_requires=[],
     cmdclass = {'build_py' : build_py_ext_first, 'sdist' : sdist_ext_first},
 )
```

### Comparing `odroid_wiringpi-3.7/wiringpi-class.py` & `odroid_wiringpi-3.8/wiringpi-class.py`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/wiringpi.i` & `odroid_wiringpi-3.8/wiringpi.i`

 * *Files identical despite different names*

### Comparing `odroid_wiringpi-3.7/wiringpi_wrap.c` & `odroid_wiringpi-3.8/wiringpi_wrap.c`

 * *Files identical despite different names*

