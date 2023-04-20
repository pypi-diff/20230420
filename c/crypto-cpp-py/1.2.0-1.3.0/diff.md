# Comparing `tmp/crypto_cpp_py-1.2.0.tar.gz` & `tmp/crypto_cpp_py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_cpp_py-1.2.0.tar", last modified: Fri Feb  3 13:09:14 2023, max compression
+gzip compressed data, was "crypto_cpp_py-1.3.0.tar", last modified: Thu Apr 20 13:24:54 2023, max compression
```

## Comparing `crypto_cpp_py-1.2.0.tar` & `crypto_cpp_py-1.3.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/build_extension.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/build_extension.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.063928 crypto_cpp_py-1.2.0/crypto-cpp/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/.git
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      616 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/presubmit.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.063928 crypto_cpp_py-1.2.0/crypto-cpp/src/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.063928 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.063928 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/big_int.h
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/big_int.inl
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/big_int_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/elliptic_curve.h
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/elliptic_curve.inl
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/elliptic_curve_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/fraction_field_element.h
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/fraction_field_element.inl
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/fraction_field_element_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/prime_field_element.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/prime_field_element.h
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/prime_field_element_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.063928 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ecdsa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ecdsa.h
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ecdsa_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)   203469 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib/crypto_lib.go
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib_test.go
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/ecdsa.cc
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/ecdsa.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/crypto.js
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/test/crypto_test.js
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/test/signature_test_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/pedersen_hash.cc
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/pedersen_hash.h
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/portable_endian.h
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/pedersen_hash.cc
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/pedersen_hash.h
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/pedersen_hash_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/order.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/order.h
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/order_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/error_handling.h
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/math.h
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/math_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/prng.h
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/prng_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/test_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.063928 crypto_cpp_py-1.2.0/crypto-cpp/src/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto-cpp/src/third_party/gsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/third_party/gsl/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    77814 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto-cpp/src/third_party/gsl/gsl-lite.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto_cpp_py/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto_cpp_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/crypto_cpp_py/cpp_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-03 13:09:14.000000 crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-02-03 13:09:14.000000 crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 13:09:14.000000 crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-03 13:09:14.000000 crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-03 13:09:14.000000 crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 13:09:14.067927 crypto_cpp_py-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-02-03 13:09:13.000000 crypto_cpp_py-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.727283 crypto_cpp_py-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 13:24:54.727283 crypto_cpp_py-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/build_extension.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/build_extension.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.719282 crypto_cpp_py-1.3.0/crypto-cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      616 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/presubmit.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.719282 crypto_cpp_py-1.3.0/crypto-cpp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.719282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.719282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/big_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/big_int.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/big_int_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/elliptic_curve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/elliptic_curve.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/elliptic_curve_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/fraction_field_element.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/fraction_field_element.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/fraction_field_element_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/prime_field_element.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/prime_field_element.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/prime_field_element_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ecdsa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ecdsa.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ecdsa_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)   203469 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib/crypto_lib.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib_test.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/ecdsa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/ecdsa.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/crypto.js
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/test/crypto_test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/test/signature_test_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/pedersen_hash.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/pedersen_hash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/portable_endian.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/pedersen_hash.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/pedersen_hash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/pedersen_hash_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/order.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/order.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/order_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/error_handling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/math_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/prng.h
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/prng_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/test_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.715282 crypto_cpp_py-1.3.0/crypto-cpp/src/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto-cpp/src/third_party/gsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/third_party/gsl/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    77814 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto-cpp/src/third_party/gsl/gsl-lite.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto_cpp_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto_cpp_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto_cpp_py/cpp_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/crypto_cpp_py/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:24:54.723282 crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 13:24:54.000000 crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-20 13:24:54.000000 crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:24:54.000000 crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 13:24:54.000000 crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 13:24:54.000000 crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:24:54.727283 crypto_cpp_py-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-20 13:24:52.000000 crypto_cpp_py-1.3.0/setup.py
```

### Comparing `crypto_cpp_py-1.2.0/PKG-INFO` & `crypto_cpp_py-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: crypto_cpp_py
-Version: 1.2.0
+Version: 1.3.0
 Summary: This is a packaged crypto-cpp program
 Home-page: https://github.com/software-mansion-labs/crypto-cpp-py.git
-Author: Wojciech Szymczyk
-Author-email: wojciech.szymczyk@swmansion.com
+Author: Wojciech Szymczyk, Marcin Warchoł
+Author-email: wojciech.szymczyk@swmansion.com, marcin.warchol@swmansion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: build
 
 Crypto-cpp-py
 =============
-A python packaged `crypto-cpp <https://python-poetry.org/>`_ library, that can be used for hashing and signing messages in starknet.
+A python packaged `crypto-cpp <https://github.com/software-mansion-labs/crypto-cpp/tree/master>`_ library, that can be used for hashing and signing messages in starknet.
 
 
 Dependencies
 ------------
-- cairo-lang
+- ecdsa,
+- sympy,
 - cmake [optional, for building package from sdist; can be installed with `pip install crypto-cpp-py[build]`]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crypto_cpp_py-1.2.0/build_extension.sh` & `crypto_cpp_py-1.3.0/build_extension.sh`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/.clang-tidy` & `crypto_cpp_py-1.3.0/crypto-cpp/.clang-tidy`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/CMakeLists.txt` & `crypto_cpp_py-1.3.0/crypto-cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/LICENSE` & `crypto_cpp_py-1.3.0/crypto-cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/presubmit.sh` & `crypto_cpp_py-1.3.0/crypto-cpp/presubmit.sh`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/CMakeLists.txt` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/big_int.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/big_int.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/big_int.inl` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/big_int.inl`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/big_int_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/big_int_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/elliptic_curve.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/elliptic_curve.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/elliptic_curve.inl` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/elliptic_curve.inl`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/elliptic_curve_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/elliptic_curve_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/fraction_field_element.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/fraction_field_element.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/fraction_field_element.inl` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/fraction_field_element.inl`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/fraction_field_element_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/fraction_field_element_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/prime_field_element.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/prime_field_element.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/prime_field_element.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/prime_field_element.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/algebra/prime_field_element_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/algebra/prime_field_element_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/CMakeLists.txt` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ecdsa.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ecdsa.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ecdsa.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ecdsa.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ecdsa_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ecdsa_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/elliptic_curve_constants_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/CMakeLists.txt` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib/crypto_lib.go` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib/crypto_lib.go`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib_test.go` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/crypto_lib_test.go`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/ecdsa.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/ecdsa.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/crypto.js` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/crypto.js`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/test/crypto_test.js` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/test/crypto_test.js`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/js/test/signature_test_data.json` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/js/test/signature_test_data.json`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/pedersen_hash.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/pedersen_hash.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/portable_endian.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/portable_endian.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/utils.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/utils.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/ffi/utils.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/ffi/utils.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/pedersen_hash.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/pedersen_hash.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/pedersen_hash.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/pedersen_hash.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/crypto/pedersen_hash_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/crypto/pedersen_hash_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/order.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/order.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/order.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/order.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/starkex/order_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/starkex/order_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/error_handling.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/error_handling.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/math.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/math.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/math_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/math_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/prng.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/prng.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/prng_test.cc` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/prng_test.cc`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/starkware/utils/test_utils.h` & `crypto_cpp_py-1.3.0/crypto-cpp/src/starkware/utils/test_utils.h`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/third_party/gsl/LICENSE` & `crypto_cpp_py-1.3.0/crypto-cpp/src/third_party/gsl/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto-cpp/src/third_party/gsl/gsl-lite.hpp` & `crypto_cpp_py-1.3.0/crypto-cpp/src/third_party/gsl/gsl-lite.hpp`

 * *Files identical despite different names*

### Comparing `crypto_cpp_py-1.2.0/crypto_cpp_py/cpp_bindings.py` & `crypto_cpp_py-1.3.0/crypto_cpp_py/cpp_bindings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ctypes
 import os
 from pathlib import Path
 from typing import Optional, Tuple
 
-from starkware.crypto.signature.signature import inv_mod_curve_size, generate_k_rfc6979
+from crypto_cpp_py.utils import cpp_generate_k_rfc6979, cpp_inv_mod_curve_size
 
 CPP_LIB_BINDING = None
 OUT_BUFFER_SIZE = 1024
 
 
 def unload_cpp_lib():
     # pylint: disable=global-statement
@@ -109,22 +109,22 @@
         raise ValueError(res.raw.rstrip(b"\00"))
     return int.from_bytes(res.raw[:32], "little", signed=False)
 
 
 def cpp_sign(msg_hash, priv_key, seed: Optional[int] = 32) -> ECSignature:
     load_cpp_lib()
     res = ctypes.create_string_buffer(OUT_BUFFER_SIZE)
-    k = generate_k_rfc6979(msg_hash, priv_key, seed)
+    k = cpp_generate_k_rfc6979(msg_hash, priv_key, seed)
     if (
         CPP_LIB_BINDING.Sign(
             priv_key.to_bytes(32, "little", signed=False),
             msg_hash.to_bytes(32, "little", signed=False),
             k.to_bytes(32, "little", signed=False),
             res,
         )
         != 0
     ):
         raise ValueError(res.raw.rstrip(b"\00"))
     # pylint: disable=invalid-name
     w = int.from_bytes(res.raw[32:64], "little", signed=False)
-    s = inv_mod_curve_size(w)
+    s = cpp_inv_mod_curve_size(w)
     return int.from_bytes(res.raw[:32], "little", signed=False), s
```

### Comparing `crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/PKG-INFO` & `crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: crypto-cpp-py
-Version: 1.2.0
+Version: 1.3.0
 Summary: This is a packaged crypto-cpp program
 Home-page: https://github.com/software-mansion-labs/crypto-cpp-py.git
-Author: Wojciech Szymczyk
-Author-email: wojciech.szymczyk@swmansion.com
+Author: Wojciech Szymczyk, Marcin Warchoł
+Author-email: wojciech.szymczyk@swmansion.com, marcin.warchol@swmansion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: build
 
 Crypto-cpp-py
 =============
-A python packaged `crypto-cpp <https://python-poetry.org/>`_ library, that can be used for hashing and signing messages in starknet.
+A python packaged `crypto-cpp <https://github.com/software-mansion-labs/crypto-cpp/tree/master>`_ library, that can be used for hashing and signing messages in starknet.
 
 
 Dependencies
 ------------
-- cairo-lang
+- ecdsa,
+- sympy,
 - cmake [optional, for building package from sdist; can be installed with `pip install crypto-cpp-py[build]`]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `crypto_cpp_py-1.2.0/crypto_cpp_py.egg-info/SOURCES.txt` & `crypto_cpp_py-1.3.0/crypto_cpp_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,12 +63,13 @@
 ./crypto-cpp/src/starkware/utils/prng.h
 ./crypto-cpp/src/starkware/utils/prng_test.cc
 ./crypto-cpp/src/starkware/utils/test_utils.h
 ./crypto-cpp/src/third_party/gsl/LICENSE
 ./crypto-cpp/src/third_party/gsl/gsl-lite.hpp
 crypto_cpp_py/__init__.py
 crypto_cpp_py/cpp_bindings.py
+crypto_cpp_py/utils.py
 crypto_cpp_py.egg-info/PKG-INFO
 crypto_cpp_py.egg-info/SOURCES.txt
 crypto_cpp_py.egg-info/dependency_links.txt
 crypto_cpp_py.egg-info/requires.txt
 crypto_cpp_py.egg-info/top_level.txt
```

### Comparing `crypto_cpp_py-1.2.0/setup.py` & `crypto_cpp_py-1.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import subprocess
 import os
+import subprocess
+
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 
 
 class CryptoExtension(Extension):
     def __init__(self):
@@ -38,32 +39,28 @@
             ) as process:
                 process.wait()
                 if process.returncode != 0:
                     raise Exception("Build returned a non-zero code")
 
         self.already_built = True
 
+
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="crypto_cpp_py",
-    version="1.2.0",
+    version="1.3.0",
     description="This is a packaged crypto-cpp program",
-    author="Wojciech Szymczyk",
-    author_email="wojciech.szymczyk@swmansion.com",
+    author="Wojciech Szymczyk, Marcin Warchoł",
+    author_email="wojciech.szymczyk@swmansion.com, marcin.warchol@swmansion.com",
     url="https://github.com/software-mansion-labs/crypto-cpp-py.git",
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    install_requires=["cairo_lang"],
+    install_requires=["ecdsa==0.18.0", "sympy==1.11.1"],
     extras_require={"build": ["cmake>=3.22.4"]},
     ext_modules=[CryptoExtension()],
-    cmdclass={
-        "build_py": BuildPy,
-        "build_ext": BuildCrypto
-    },
+    cmdclass={"build_py": BuildPy, "build_ext": BuildCrypto},
     python_requires=">=3.8",
     packages=["crypto_cpp_py"],
-    package_data={
-        "crypto_cpp_py": ["../libcrypto_c_exports.*"]
-    }
+    package_data={"crypto_cpp_py": ["../libcrypto_c_exports.*"]},
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

