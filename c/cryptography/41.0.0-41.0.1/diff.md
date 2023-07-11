# Comparing `tmp/cryptography-41.0.0.tar.gz` & `tmp/cryptography-41.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptography-41.0.0.tar", last modified: Tue May 30 21:37:39 2023, max compression
+gzip compressed data, was "cryptography-41.0.1.tar", last modified: Thu Jun  1 12:20:37 2023, max compression
```

## Comparing `cryptography-41.0.0.tar` & `cryptography-41.0.1.tar`

### file list

```diff
@@ -1,431 +1,431 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.161162 cryptography-41.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    91024 2023-05-30 21:37:26.000000 cryptography-41.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 21:37:26.000000 cryptography-41.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 21:37:26.000000 cryptography-41.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-30 21:37:26.000000 cryptography-41.0.0/LICENSE.APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-30 21:37:26.000000 cryptography-41.0.0/LICENSE.BSD
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-30 21:37:26.000000 cryptography-41.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-30 21:37:39.161162 cryptography-41.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-30 21:37:26.000000 cryptography-41.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/_ext/cryptography-docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/_ext/linkcode_res.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/api-stability.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/community.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/development/
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/c-bindings.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/arc4/
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/arc4/generate_arc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/arc4/verify_arc4.go
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/arc4.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/cast5/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/cast5/generate_cast5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/cast5/verify_cast5.go
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/cast5.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/hkdf/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/hkdf/generate_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/hkdf/verify_hkdf.go
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/hkdf.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/idea/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/idea/generate_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/idea/verify_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/idea.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/
--rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/secp256k1/
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/secp256k1/generate_secp256k1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/secp256k1/verify_secp256k1.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/secp256k1.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/seed/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/seed/generate_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/seed/verify_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/seed.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/reviewing-patches.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/submitting-patches.rst
--rw-r--r--   0 runner    (1001) docker     (123)    58752 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/test-vectors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/doing-a-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/fernet.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.093161 cryptography-41.0.0/docs/hazmat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/aead.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dh.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dsa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28533 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed25519.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed448.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26600 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/rsa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    56191 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/serialization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x25519.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x448.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/constant-time.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/cryptographic-hashes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44313 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/key-derivation-functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/keywrap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/docs/hazmat/primitives/mac/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/cmac.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/hmac.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/poly1305.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/padding.rst
--rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/symmetric-encryption.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/twofactor.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/openssl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/random-numbers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/security.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/docs/x509/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/certificate-transparency.rst
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29766 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/ocsp.rst
--rw-r--r--   0 runner    (1001) docker     (123)   127728 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-30 21:37:26.000000 cryptography-41.0.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-30 21:37:26.000000 cryptography-41.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:37:39.161162 cryptography-41.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-30 21:37:26.000000 cryptography-41.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.093161 cryptography-41.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/src/_cffi_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/build_openssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/_cffi_src/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/bignum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/bio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/dh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/err.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/evp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/evp_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/fips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/nid.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/opensslv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509_vfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/fernet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography/hazmat/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/_oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography/hazmat/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.121162 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/aead.py
--rw-r--r--   0 runner    (1001) docker     (123)    73231 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ciphers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/decode_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21825 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.121162 cryptography-41.0.0/src/cryptography/hazmat/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.121162 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/_openssl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/asn1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/ocsp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.125162 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/x509.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.125162 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.125162 cryptography-41.0.0/src/cryptography/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/_asymmetric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/_cipheralgorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ed25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ed448.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x448.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/aead.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/constant_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/hmac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/concatkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/kbkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/scrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/x963kdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/keywrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/poly1305.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)    50088 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/hotp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/totp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/cryptography/x509/
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35677 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/certificate_transparency.py
--rw-r--r--   0 runner    (1001) docker     (123)    68365 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/general_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/ocsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:37:38.000000 cryptography-41.0.0/src/cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-cffi/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-cffi/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-cffi/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-cffi/src/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-cffi/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-openssl/src/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/src/fips.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/src/hmac.rs
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-x509/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.137162 cryptography-41.0.0/src/rust/cryptography-x509/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/certificate.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/common.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/crl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/csr.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/extensions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/name.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/ocsp_req.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/ocsp_resp.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/oid.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/pkcs7.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.137162 cryptography-41.0.0/src/rust/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/asn1.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.141162 cryptography-41.0.0/src/rust/src/backend/
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/dh.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/dsa.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/ed25519.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/ed448.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/hashes.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/hmac.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/kdf.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/poly1305.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/x25519.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/x448.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/buf.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/exceptions.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/oid.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/pkcs7.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/pool.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.141162 cryptography-41.0.0/src/rust/src/x509/
--rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/certificate.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/common.rs
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/crl.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/csr.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/extensions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/ocsp.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/ocsp_req.rs
--rw-r--r--   0 runner    (1001) docker     (123)    30555 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/ocsp_resp.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/sct.rs
--rw-r--r--   0 runner    (1001) docker     (123)    29557 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/sign.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_ec_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_x509.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/deprecated_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/doubles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/hazmat/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/hazmat/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/backends/test_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/backends/test_openssl_memleak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/hazmat/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/bindings/test_openssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.157162 cryptography-41.0.0/tests/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_dh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_3des.py
--rw-r--r--   0 runner    (1001) docker     (123)    26688 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_aes_gcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_arc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_asym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_cast5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ciphers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_concatkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_constant_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    36819 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_dh.py
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    46372 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ed25519.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ed448.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hash_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hkdf_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hmac_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)    26335 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_kbkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_kbkdf_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_keywrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_poly1305.py
--rw-r--r--   0 runner    (1001) docker     (123)    99908 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_scrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    55019 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_sm4.py
--rw-r--r--   0 runner    (1001) docker     (123)    69339 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x448.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x963_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x963kdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.157162 cryptography-41.0.0/tests/hazmat/primitives/twofactor/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/twofactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_hotp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/test_oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_cryptography_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_fernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   188472 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    29807 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.161162 cryptography-41.0.0/tests/wycheproof/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_chacha20poly1305.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_ecdh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_keywrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_x448.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.161162 cryptography-41.0.0/tests/x509/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    53924 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_ocsp.py
--rw-r--r--   0 runner    (1001) docker     (123)   244850 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509.py
--rw-r--r--   0 runner    (1001) docker     (123)    31158 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509_crlbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)   218778 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509_revokedcertbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.477401 cryptography-41.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    91283 2023-06-01 12:20:23.000000 cryptography-41.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-01 12:20:23.000000 cryptography-41.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-01 12:20:23.000000 cryptography-41.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-01 12:20:23.000000 cryptography-41.0.1/LICENSE.APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-01 12:20:23.000000 cryptography-41.0.1/LICENSE.BSD
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-01 12:20:23.000000 cryptography-41.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-01 12:20:37.477401 cryptography-41.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-01 12:20:23.000000 cryptography-41.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/_ext/cryptography-docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/_ext/linkcode_res.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/api-stability.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/community.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/c-bindings.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/development/custom-vectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/development/custom-vectors/arc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/arc4/generate_arc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/arc4/verify_arc4.go
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/arc4.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/development/custom-vectors/cast5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/cast5/generate_cast5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/cast5/verify_cast5.go
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/cast5.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/development/custom-vectors/hkdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/hkdf/generate_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/hkdf/verify_hkdf.go
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/hkdf.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.425400 cryptography-41.0.1/docs/development/custom-vectors/idea/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/idea/generate_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/idea/verify_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/idea.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.429400 cryptography-41.0.1/docs/development/custom-vectors/rsa-oaep-sha2/
+-rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/rsa-oaep-sha2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.429400 cryptography-41.0.1/docs/development/custom-vectors/secp256k1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/secp256k1/generate_secp256k1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/secp256k1/verify_secp256k1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/secp256k1.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.429400 cryptography-41.0.1/docs/development/custom-vectors/seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/seed/generate_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/seed/verify_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/custom-vectors/seed.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/reviewing-patches.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/submitting-patches.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    58911 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/development/test-vectors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/doing-a-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/fernet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.417400 cryptography-41.0.1/docs/hazmat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.429400 cryptography-41.0.1/docs/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/aead.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.429400 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/dh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/dsa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28533 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/ec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/ed25519.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/ed448.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26600 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/rsa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    56191 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/x25519.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/asymmetric/x448.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/constant-time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/cryptographic-hashes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44313 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/key-derivation-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/keywrap.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.433400 cryptography-41.0.1/docs/hazmat/primitives/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/mac/cmac.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/mac/hmac.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/mac/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/mac/poly1305.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/padding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/symmetric-encryption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/hazmat/primitives/twofactor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/openssl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/random-numbers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/security.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/spelling_wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.433400 cryptography-41.0.1/docs/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/x509/certificate-transparency.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/x509/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29766 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/x509/ocsp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   127728 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/x509/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-01 12:20:23.000000 cryptography-41.0.1/docs/x509/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-01 12:20:23.000000 cryptography-41.0.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-01 12:20:23.000000 cryptography-41.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:20:37.477401 cryptography-41.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-01 12:20:23.000000 cryptography-41.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.421400 cryptography-41.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.433400 cryptography-41.0.1/src/_cffi_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/build_openssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.437400 cryptography-41.0.1/src/_cffi_src/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/bignum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/bio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/err.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/evp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/evp_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/fips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/nid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/opensslv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/x509_vfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/x509name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/openssl/x509v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/_cffi_src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.437400 cryptography-41.0.1/src/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/fernet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.437400 cryptography-41.0.1/src/cryptography/hazmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/_oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.437400 cryptography-41.0.1/src/cryptography/hazmat/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.437400 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73231 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/ciphers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/decode_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21825 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.437400 cryptography-41.0.1/src/cryptography/hazmat/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.441400 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/_openssl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/asn1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/ocsp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.441400 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/x509.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.441400 cryptography-41.0.1/src/cryptography/hazmat/bindings/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/openssl/_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/bindings/openssl/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.441400 cryptography-41.0.1/src/cryptography/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/_asymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/_cipheralgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.445400 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/ed448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/x448.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.445400 cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/constant_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/hmac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.445400 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/concatkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/kbkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/x963kdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/poly1305.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.445400 cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50088 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.445400 cryptography-41.0.1/src/cryptography/hazmat/primitives/twofactor/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/twofactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/twofactor/hotp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/hazmat/primitives/twofactor/totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.449400 cryptography-41.0.1/src/cryptography/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35677 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/certificate_transparency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68365 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/cryptography/x509/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.437400 cryptography-41.0.1/src/cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-01 12:20:37.000000 cryptography-41.0.1/src/cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-06-01 12:20:37.000000 cryptography-41.0.1/src/cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:20:37.000000 cryptography-41.0.1/src/cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:20:37.000000 cryptography-41.0.1/src/cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-01 12:20:37.000000 cryptography-41.0.1/src/cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 12:20:37.000000 cryptography-41.0.1/src/cryptography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.449400 cryptography-41.0.1/src/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.449400 cryptography-41.0.1/src/rust/cryptography-cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-cffi/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-cffi/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.449400 cryptography-41.0.1/src/rust/cryptography-cffi/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-cffi/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.449400 cryptography-41.0.1/src/rust/cryptography-openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-openssl/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-openssl/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.453400 cryptography-41.0.1/src/rust/cryptography-openssl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-openssl/src/fips.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-openssl/src/hmac.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-openssl/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.453400 cryptography-41.0.1/src/rust/cryptography-x509/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.453400 cryptography-41.0.1/src/rust/cryptography-x509/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/common.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/crl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/csr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/extensions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/ocsp_req.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/ocsp_resp.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/oid.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/cryptography-x509/src/pkcs7.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.453400 cryptography-41.0.1/src/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/asn1.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.457400 cryptography-41.0.1/src/rust/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/dh.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/dsa.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/ed25519.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/ed448.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/hashes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/hmac.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/kdf.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/poly1305.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/x25519.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/backend/x448.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/buf.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/exceptions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/oid.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/pkcs7.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/pool.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.461400 cryptography-41.0.1/src/rust/src/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)    38268 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/common.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/crl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/csr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/extensions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/ocsp.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/ocsp_req.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    30555 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/ocsp_resp.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/sct.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-06-01 12:20:23.000000 cryptography-41.0.1/src/rust/src/x509/sign.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.465401 cryptography-41.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.465401 cryptography-41.0.1/tests/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/bench/test_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/bench/test_ec_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/bench/test_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/bench/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/bench/test_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/deprecated_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/doubles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.465401 cryptography-41.0.1/tests/hazmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.465401 cryptography-41.0.1/tests/hazmat/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/backends/test_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/backends/test_openssl_memleak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.465401 cryptography-41.0.1/tests/hazmat/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/bindings/test_openssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.473400 cryptography-41.0.1/tests/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/fixtures_dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/fixtures_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/fixtures_ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/fixtures_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_3des.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26688 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_aes_gcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_arc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_asym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_cast5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_ciphers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_concatkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_constant_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36819 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46372 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_ed448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_hash_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_hkdf_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_hmac_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26335 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_kbkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_kbkdf_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_pbkdf2hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_poly1305.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99908 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55019 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_sm4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69339 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_x448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_x963_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/test_x963kdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.473400 cryptography-41.0.1/tests/hazmat/primitives/twofactor/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/twofactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/twofactor/test_hotp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/twofactor/test_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/hazmat/test_oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/test_cryptography_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/test_fernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/test_rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188472 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29807 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.477401 cryptography-41.0.1/tests/wycheproof/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_chacha20poly1305.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_ecdh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/test_x448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/wycheproof/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:37.477401 cryptography-41.0.1/tests/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/x509/test_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53924 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/x509/test_ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245594 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/x509/test_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31158 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/x509/test_x509_crlbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)   218778 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/x509/test_x509_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-01 12:20:23.000000 cryptography-41.0.1/tests/x509/test_x509_revokedcertbuilder.py
```

### Comparing `cryptography-41.0.0/CHANGELOG.rst` & `cryptography-41.0.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+.. _v41-0-1:
+
+41.0.1 - 2023-06-01
+~~~~~~~~~~~~~~~~~~~
+
+* Temporarily allow invalid ECDSA signature algorithm parameters in X.509
+  certificates, which are generated by older versions of Java.
+* Allow null bytes in pass phrases when serializing private keys.
+
 .. _v41-0-0:
 
 41.0.0 - 2023-05-30
 ~~~~~~~~~~~~~~~~~~~
 
 * **BACKWARDS INCOMPATIBLE:** Support for OpenSSL less than 1.1.1d has been
   removed.  Users on older version of OpenSSL will need to upgrade.
```

### Comparing `cryptography-41.0.0/CONTRIBUTING.rst` & `cryptography-41.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/LICENSE.APACHE` & `cryptography-41.0.1/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/LICENSE.BSD` & `cryptography-41.0.1/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/MANIFEST.in` & `cryptography-41.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/PKG-INFO` & `cryptography-41.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography
-Version: 41.0.0
+Version: 41.0.1
 Summary: cryptography is a package which provides cryptographic recipes and primitives to Python developers.
 Author-email: The Python Cryptographic Authority and individual contributors <cryptography-dev@python.org>
 License: Apache-2.0 OR BSD-3-Clause
 Project-URL: homepage, https://github.com/pyca/cryptography
 Project-URL: documentation, https://cryptography.io/
 Project-URL: source, https://github.com/pyca/cryptography/
 Project-URL: issues, https://github.com/pyca/cryptography/issues
```

### Comparing `cryptography-41.0.0/README.rst` & `cryptography-41.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/Makefile` & `cryptography-41.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/_ext/cryptography-docs.py` & `cryptography-41.0.1/docs/_ext/cryptography-docs.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/_ext/linkcode_res.py` & `cryptography-41.0.1/docs/_ext/linkcode_res.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/api-stability.rst` & `cryptography-41.0.1/docs/api-stability.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/community.rst` & `cryptography-41.0.1/docs/community.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/conf.py` & `cryptography-41.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/c-bindings.rst` & `cryptography-41.0.1/docs/development/c-bindings.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/arc4/generate_arc4.py` & `cryptography-41.0.1/docs/development/custom-vectors/arc4/generate_arc4.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/arc4/verify_arc4.go` & `cryptography-41.0.1/docs/development/custom-vectors/arc4/verify_arc4.go`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/arc4.rst` & `cryptography-41.0.1/docs/development/custom-vectors/arc4.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/cast5/generate_cast5.py` & `cryptography-41.0.1/docs/development/custom-vectors/cast5/generate_cast5.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/cast5/verify_cast5.go` & `cryptography-41.0.1/docs/development/custom-vectors/cast5/verify_cast5.go`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/cast5.rst` & `cryptography-41.0.1/docs/development/custom-vectors/cast5.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/hkdf/generate_hkdf.py` & `cryptography-41.0.1/docs/development/custom-vectors/hkdf/generate_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/hkdf/verify_hkdf.go` & `cryptography-41.0.1/docs/development/custom-vectors/hkdf/verify_hkdf.go`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/hkdf.rst` & `cryptography-41.0.1/docs/development/custom-vectors/hkdf.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/idea/generate_idea.py` & `cryptography-41.0.1/docs/development/custom-vectors/idea/generate_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/idea/verify_idea.py` & `cryptography-41.0.1/docs/development/custom-vectors/idea/verify_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/idea.rst` & `cryptography-41.0.1/docs/development/custom-vectors/idea.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java` & `cryptography-41.0.1/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py` & `cryptography-41.0.1/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2.rst` & `cryptography-41.0.1/docs/development/custom-vectors/rsa-oaep-sha2.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/secp256k1/generate_secp256k1.py` & `cryptography-41.0.1/docs/development/custom-vectors/secp256k1/generate_secp256k1.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/secp256k1/verify_secp256k1.py` & `cryptography-41.0.1/docs/development/custom-vectors/secp256k1/verify_secp256k1.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/secp256k1.rst` & `cryptography-41.0.1/docs/development/custom-vectors/secp256k1.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/seed/generate_seed.py` & `cryptography-41.0.1/docs/development/custom-vectors/seed/generate_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/seed/verify_seed.py` & `cryptography-41.0.1/docs/development/custom-vectors/seed/verify_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/custom-vectors/seed.rst` & `cryptography-41.0.1/docs/development/custom-vectors/seed.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/getting-started.rst` & `cryptography-41.0.1/docs/development/getting-started.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/index.rst` & `cryptography-41.0.1/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/reviewing-patches.rst` & `cryptography-41.0.1/docs/development/reviewing-patches.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/submitting-patches.rst` & `cryptography-41.0.1/docs/development/submitting-patches.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/development/test-vectors.rst` & `cryptography-41.0.1/docs/development/test-vectors.rst`

 * *Files 1% similar despite different names*

```diff
@@ -495,14 +495,16 @@
   ``x509/cryptography.io.pem`` but modifying the ``tbs_cert.signature_algorithm``
   OID to not match the outer signature algorithm OID.
 * ``ms-certificate-template.pem`` - A certificate with a ``msCertificateTemplate``
   extension.
 * ``rsa_pss_sha256_no_null.pem`` - A certificate with an RSA PSS signature
   with no encoded ``NULL`` for the PSS hash algorithm parameters. This certificate
   was generated by LibreSSL.
+* ``ecdsa_null_alg.pem`` - A certificate with an ECDSA signature with ``NULL``
+  algorithm parameters. This encoding is invalid, but was generated by Java 11.
 
 Custom X.509 Request Vectors
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * ``dsa_sha1.pem`` and ``dsa_sha1.der`` - Contain a certificate request using
   1024-bit DSA parameters and SHA1 generated using OpenSSL.
 * ``rsa_md4.pem`` and ``rsa_md4.der`` - Contain a certificate request using
```

### Comparing `cryptography-41.0.0/docs/doing-a-release.rst` & `cryptography-41.0.1/docs/doing-a-release.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/exceptions.rst` & `cryptography-41.0.1/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/faq.rst` & `cryptography-41.0.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/fernet.rst` & `cryptography-41.0.1/docs/fernet.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/glossary.rst` & `cryptography-41.0.1/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/aead.rst` & `cryptography-41.0.1/docs/hazmat/primitives/aead.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dh.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/dh.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dsa.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/dsa.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ec.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/ec.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed25519.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/ed25519.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed448.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/ed448.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/index.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/rsa.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/rsa.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/serialization.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/serialization.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/utils.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/utils.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x25519.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/x25519.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x448.rst` & `cryptography-41.0.1/docs/hazmat/primitives/asymmetric/x448.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/constant-time.rst` & `cryptography-41.0.1/docs/hazmat/primitives/constant-time.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/cryptographic-hashes.rst` & `cryptography-41.0.1/docs/hazmat/primitives/cryptographic-hashes.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/key-derivation-functions.rst` & `cryptography-41.0.1/docs/hazmat/primitives/key-derivation-functions.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/keywrap.rst` & `cryptography-41.0.1/docs/hazmat/primitives/keywrap.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/mac/cmac.rst` & `cryptography-41.0.1/docs/hazmat/primitives/mac/cmac.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/mac/hmac.rst` & `cryptography-41.0.1/docs/hazmat/primitives/mac/hmac.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/mac/poly1305.rst` & `cryptography-41.0.1/docs/hazmat/primitives/mac/poly1305.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/padding.rst` & `cryptography-41.0.1/docs/hazmat/primitives/padding.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/symmetric-encryption.rst` & `cryptography-41.0.1/docs/hazmat/primitives/symmetric-encryption.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/hazmat/primitives/twofactor.rst` & `cryptography-41.0.1/docs/hazmat/primitives/twofactor.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/index.rst` & `cryptography-41.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/installation.rst` & `cryptography-41.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/limitations.rst` & `cryptography-41.0.1/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/make.bat` & `cryptography-41.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/openssl.rst` & `cryptography-41.0.1/docs/openssl.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/random-numbers.rst` & `cryptography-41.0.1/docs/random-numbers.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/security.rst` & `cryptography-41.0.1/docs/security.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/spelling_wordlist.txt` & `cryptography-41.0.1/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/x509/certificate-transparency.rst` & `cryptography-41.0.1/docs/x509/certificate-transparency.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/x509/ocsp.rst` & `cryptography-41.0.1/docs/x509/ocsp.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/x509/reference.rst` & `cryptography-41.0.1/docs/x509/reference.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/docs/x509/tutorial.rst` & `cryptography-41.0.1/docs/x509/tutorial.rst`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/noxfile.py` & `cryptography-41.0.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/pyproject.toml` & `cryptography-41.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "cffi>=1.12; platform_python_implementation != 'PyPy'",
     "setuptools-rust>=0.11.4",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cryptography"
-version = "41.0.0"
+version = "41.0.1"
 authors = [
     {name = "The Python Cryptographic Authority and individual contributors", email = "cryptography-dev@python.org"}
 ]
 description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
 readme = "README.rst"
 license = {text = "Apache-2.0 OR BSD-3-Clause"}
 classifiers = [
```

### Comparing `cryptography-41.0.0/setup.py` & `cryptography-41.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/build_openssl.py` & `cryptography-41.0.1/src/_cffi_src/build_openssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/asn1.py` & `cryptography-41.0.1/src/_cffi_src/openssl/asn1.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/bignum.py` & `cryptography-41.0.1/src/_cffi_src/openssl/bignum.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/bio.py` & `cryptography-41.0.1/src/_cffi_src/openssl/bio.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/callbacks.py` & `cryptography-41.0.1/src/_cffi_src/openssl/callbacks.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/cmac.py` & `cryptography-41.0.1/src/_cffi_src/openssl/cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/crypto.py` & `cryptography-41.0.1/src/_cffi_src/openssl/crypto.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/cryptography.py` & `cryptography-41.0.1/src/_cffi_src/openssl/cryptography.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/dsa.py` & `cryptography-41.0.1/src/_cffi_src/openssl/dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/ec.py` & `cryptography-41.0.1/src/_cffi_src/openssl/ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/ecdsa.py` & `cryptography-41.0.1/src/_cffi_src/openssl/ecdsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/engine.py` & `cryptography-41.0.1/src/_cffi_src/openssl/engine.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/err.py` & `cryptography-41.0.1/src/_cffi_src/openssl/err.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/evp.py` & `cryptography-41.0.1/src/_cffi_src/openssl/evp.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/evp_aead.py` & `cryptography-41.0.1/src/_cffi_src/openssl/evp_aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/fips.py` & `cryptography-41.0.1/src/_cffi_src/openssl/fips.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/nid.py` & `cryptography-41.0.1/src/_cffi_src/openssl/nid.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/opensslv.py` & `cryptography-41.0.1/src/_cffi_src/openssl/opensslv.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/pem.py` & `cryptography-41.0.1/src/_cffi_src/openssl/pem.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/pkcs12.py` & `cryptography-41.0.1/src/_cffi_src/openssl/pkcs12.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/pkcs7.py` & `cryptography-41.0.1/src/_cffi_src/openssl/pkcs7.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/provider.py` & `cryptography-41.0.1/src/_cffi_src/openssl/provider.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/rsa.py` & `cryptography-41.0.1/src/_cffi_src/openssl/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/ssl.py` & `cryptography-41.0.1/src/_cffi_src/openssl/ssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/x509.py` & `cryptography-41.0.1/src/_cffi_src/openssl/x509.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/x509_vfy.py` & `cryptography-41.0.1/src/_cffi_src/openssl/x509_vfy.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/x509name.py` & `cryptography-41.0.1/src/_cffi_src/openssl/x509name.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/openssl/x509v3.py` & `cryptography-41.0.1/src/_cffi_src/openssl/x509v3.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/_cffi_src/utils.py` & `cryptography-41.0.1/src/_cffi_src/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/exceptions.py` & `cryptography-41.0.1/src/cryptography/exceptions.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/fernet.py` & `cryptography-41.0.1/src/cryptography/fernet.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/_oid.py` & `cryptography-41.0.1/src/cryptography/hazmat/_oid.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/aead.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/backend.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/backend.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ciphers.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/cmac.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/decode_asn1.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/decode_asn1.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ec.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/rsa.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/utils.py` & `cryptography-41.0.1/src/cryptography/hazmat/backends/openssl/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/__init__.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/asn1.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/asn1.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/exceptions.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/ocsp.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/x509.pyi` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/_rust/x509.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/_conditional.py` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/openssl/_conditional.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/binding.py` & `cryptography-41.0.1/src/cryptography/hazmat/bindings/openssl/binding.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/_asymmetric.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/_asymmetric.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/_cipheralgorithm.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/_cipheralgorithm.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/_serialization.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/_serialization.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dh.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/dh.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dsa.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ec.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ed25519.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/ed25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ed448.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/ed448.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/padding.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/padding.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/rsa.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/types.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/types.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/utils.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x25519.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/x25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x448.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/asymmetric/x448.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/__init__.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/aead.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/algorithms.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/algorithms.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/base.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/base.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/modes.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/ciphers/modes.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/cmac.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/hashes.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/hashes.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/__init__.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/concatkdf.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/concatkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/hkdf.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/kbkdf.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/kbkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/pbkdf2.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/scrypt.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/scrypt.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/x963kdf.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/kdf/x963kdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/keywrap.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/padding.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/padding.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/__init__.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/base.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/base.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs12.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/pkcs12.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs7.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/pkcs7.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/ssh.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/serialization/ssh.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/hotp.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/twofactor/hotp.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/totp.py` & `cryptography-41.0.1/src/cryptography/hazmat/primitives/twofactor/totp.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/utils.py` & `cryptography-41.0.1/src/cryptography/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/__init__.py` & `cryptography-41.0.1/src/cryptography/x509/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/base.py` & `cryptography-41.0.1/src/cryptography/x509/base.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/certificate_transparency.py` & `cryptography-41.0.1/src/cryptography/x509/certificate_transparency.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/extensions.py` & `cryptography-41.0.1/src/cryptography/x509/extensions.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/general_name.py` & `cryptography-41.0.1/src/cryptography/x509/general_name.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/name.py` & `cryptography-41.0.1/src/cryptography/x509/name.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/ocsp.py` & `cryptography-41.0.1/src/cryptography/x509/ocsp.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography/x509/oid.py` & `cryptography-41.0.1/src/cryptography/x509/oid.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/cryptography.egg-info/PKG-INFO` & `cryptography-41.0.1/src/cryptography.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography
-Version: 41.0.0
+Version: 41.0.1
 Summary: cryptography is a package which provides cryptographic recipes and primitives to Python developers.
 Author-email: The Python Cryptographic Authority and individual contributors <cryptography-dev@python.org>
 License: Apache-2.0 OR BSD-3-Clause
 Project-URL: homepage, https://github.com/pyca/cryptography
 Project-URL: documentation, https://cryptography.io/
 Project-URL: source, https://github.com/pyca/cryptography/
 Project-URL: issues, https://github.com/pyca/cryptography/issues
```

### Comparing `cryptography-41.0.0/src/cryptography.egg-info/SOURCES.txt` & `cryptography-41.0.1/src/cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/Cargo.lock` & `cryptography-41.0.1/src/rust/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -158,17 +158,17 @@
 name = "once_cell"
 version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "openssl"
-version = "0.10.53"
+version = "0.10.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12df40a956736488b7b44fe79fe12d4f245bb5b3f5a1f6095e499760015be392"
+checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
```

### Comparing `cryptography-41.0.0/src/rust/Cargo.toml` & `cryptography-41.0.1/src/rust/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pyo3 = { version = "0.18", features = ["abi3-py37"] }
 asn1 = { version = "0.15.2", default-features = false }
 cryptography-cffi = { path = "cryptography-cffi" }
 cryptography-x509 = { path = "cryptography-x509" }
 cryptography-openssl = { path = "cryptography-openssl" }
 pem = "1.1"
 ouroboros = "0.15"
-openssl = "0.10.53"
+openssl = "0.10.54"
 openssl-sys = "0.9.88"
 foreign-types-shared = "0.1"
 
 [build-dependencies]
 cc = "1.0.72"
 
 [features]
```

### Comparing `cryptography-41.0.0/src/rust/build.rs` & `cryptography-41.0.1/src/rust/build.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-cffi/build.rs` & `cryptography-41.0.1/src/rust/cryptography-cffi/build.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-cffi/src/lib.rs` & `cryptography-41.0.1/src/rust/cryptography-cffi/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-openssl/build.rs` & `cryptography-41.0.1/src/rust/cryptography-openssl/build.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-openssl/src/fips.rs` & `cryptography-41.0.1/src/rust/cryptography-openssl/src/fips.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-openssl/src/hmac.rs` & `cryptography-41.0.1/src/rust/cryptography-openssl/src/hmac.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-openssl/src/lib.rs` & `cryptography-41.0.1/src/rust/cryptography-openssl/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/certificate.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/certificate.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/common.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/common.rs`

 * *Files 3% similar despite different names*

```diff
@@ -41,22 +41,26 @@
     Sha3_512(Option<asn1::Null>),
 
     #[defined_by(oid::ED25519_OID)]
     Ed25519,
     #[defined_by(oid::ED448_OID)]
     Ed448,
 
+    // These ECDSA algorithms should have no parameters,
+    // but Java 11 (up to at least 11.0.19) encodes them
+    // with NULL parameters. The JDK team is looking to
+    // backport the fix as of June 2023.
     #[defined_by(oid::ECDSA_WITH_SHA224_OID)]
-    EcDsaWithSha224,
+    EcDsaWithSha224(Option<asn1::Null>),
     #[defined_by(oid::ECDSA_WITH_SHA256_OID)]
-    EcDsaWithSha256,
+    EcDsaWithSha256(Option<asn1::Null>),
     #[defined_by(oid::ECDSA_WITH_SHA384_OID)]
-    EcDsaWithSha384,
+    EcDsaWithSha384(Option<asn1::Null>),
     #[defined_by(oid::ECDSA_WITH_SHA512_OID)]
-    EcDsaWithSha512,
+    EcDsaWithSha512(Option<asn1::Null>),
 
     #[defined_by(oid::ECDSA_WITH_SHA3_224_OID)]
     EcDsaWithSha3_224,
     #[defined_by(oid::ECDSA_WITH_SHA3_256_OID)]
     EcDsaWithSha3_256,
     #[defined_by(oid::ECDSA_WITH_SHA3_384_OID)]
     EcDsaWithSha3_384,
```

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/crl.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/crl.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/csr.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/csr.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/extensions.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/extensions.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/name.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/name.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/ocsp_req.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/ocsp_req.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/ocsp_resp.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/ocsp_resp.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/oid.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/oid.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/cryptography-x509/src/pkcs7.rs` & `cryptography-41.0.1/src/rust/cryptography-x509/src/pkcs7.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/asn1.rs` & `cryptography-41.0.1/src/rust/src/asn1.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/dh.rs` & `cryptography-41.0.1/src/rust/src/backend/dh.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/dsa.rs` & `cryptography-41.0.1/src/rust/src/backend/dsa.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/ed25519.rs` & `cryptography-41.0.1/src/rust/src/backend/ed25519.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/ed448.rs` & `cryptography-41.0.1/src/rust/src/backend/ed448.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/hashes.rs` & `cryptography-41.0.1/src/rust/src/backend/hashes.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/hmac.rs` & `cryptography-41.0.1/src/rust/src/backend/hmac.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/kdf.rs` & `cryptography-41.0.1/src/rust/src/backend/kdf.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/mod.rs` & `cryptography-41.0.1/src/rust/src/backend/mod.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/poly1305.rs` & `cryptography-41.0.1/src/rust/src/backend/poly1305.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/utils.rs` & `cryptography-41.0.1/src/rust/src/backend/utils.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/x25519.rs` & `cryptography-41.0.1/src/rust/src/backend/x25519.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/backend/x448.rs` & `cryptography-41.0.1/src/rust/src/backend/x448.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/buf.rs` & `cryptography-41.0.1/src/rust/src/buf.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/error.rs` & `cryptography-41.0.1/src/rust/src/error.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/exceptions.rs` & `cryptography-41.0.1/src/rust/src/exceptions.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/lib.rs` & `cryptography-41.0.1/src/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/oid.rs` & `cryptography-41.0.1/src/rust/src/oid.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/pkcs7.rs` & `cryptography-41.0.1/src/rust/src/pkcs7.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/pool.rs` & `cryptography-41.0.1/src/rust/src/pool.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/certificate.rs` & `cryptography-41.0.1/src/rust/src/x509/certificate.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 use crate::asn1::{
     big_byte_slice_to_py_int, encode_der_data, oid_to_py_oid, py_uint_to_big_endian_bytes,
 };
 use crate::error::{CryptographyError, CryptographyResult};
 use crate::x509::{extensions, sct, sign};
 use crate::{exceptions, x509};
-use cryptography_x509::common::Asn1ReadableOrWritable;
+use cryptography_x509::common::{AlgorithmParameters, Asn1ReadableOrWritable};
 use cryptography_x509::extensions::Extension;
 use cryptography_x509::extensions::{
     AuthorityKeyIdentifier, BasicConstraints, DisplayText, DistributionPoint,
     DistributionPointName, MSCertificateTemplate, NameConstraints, PolicyConstraints,
     PolicyInformation, PolicyQualifierInfo, Qualifier, RawExtensions, SequenceOfAccessDescriptions,
     SequenceOfSubtrees, UserNotice,
 };
@@ -387,14 +387,18 @@
 ) -> CryptographyResult<Certificate> {
     let raw = OwnedCertificate::try_new(data, |data| asn1::parse_single(data.as_bytes(py)))?;
     // Parse cert version immediately so we can raise error on parse if it is invalid.
     cert_version(py, raw.borrow_value().tbs_cert.version)?;
     // determine if the serial is negative and raise a warning if it is. We want to drop support
     // for this sort of invalid encoding eventually.
     warn_if_negative_serial(py, raw.borrow_value().tbs_cert.serial.as_bytes())?;
+    // determine if the signature algorithm has incorrect parameters and raise a warning if it
+    // does. this is a bug in JDK11 and we want to drop support for it eventually.
+    warn_if_invalid_ecdsa_params(py, raw.borrow_value().signature_alg.params.clone())?;
+    warn_if_invalid_ecdsa_params(py, raw.borrow_value().tbs_cert.signature_alg.params.clone())?;
 
     Ok(Certificate {
         raw,
         cached_extensions: None,
     })
 }
 
@@ -409,14 +413,38 @@
             "Parsed a negative serial number, which is disallowed by RFC 5280.",
             1,
         )?;
     }
     Ok(())
 }
 
+fn warn_if_invalid_ecdsa_params(
+    py: pyo3::Python<'_>,
+    params: AlgorithmParameters<'_>,
+) -> pyo3::PyResult<()> {
+    match params {
+        AlgorithmParameters::EcDsaWithSha224(Some(..))
+        | AlgorithmParameters::EcDsaWithSha256(Some(..))
+        | AlgorithmParameters::EcDsaWithSha384(Some(..))
+        | AlgorithmParameters::EcDsaWithSha512(Some(..)) => {
+            let cryptography_warning = py
+                .import(pyo3::intern!(py, "cryptography.utils"))?
+                .getattr(pyo3::intern!(py, "DeprecatedIn41"))?;
+            pyo3::PyErr::warn(
+                py,
+                cryptography_warning,
+                "The parsed certificate contains a NULL parameter value in its signature algorithm parameters. This is invalid and will be rejected in a future version of cryptography. If this certificate was created via Java, please upgrade to JDK16+ or the latest JDK11 once a fix is issued. If this certificate was created in some other fashion please report the issue to the cryptography issue tracker. See https://github.com/pyca/cryptography/issues/8996 for more details.",
+                2,
+            )?;
+        }
+        _ => {}
+    }
+    Ok(())
+}
+
 fn parse_display_text(
     py: pyo3::Python<'_>,
     text: DisplayText<'_>,
 ) -> pyo3::PyResult<pyo3::PyObject> {
     match text {
         DisplayText::IA5String(o) => Ok(pyo3::types::PyString::new(py, o.as_str()).to_object(py)),
         DisplayText::Utf8String(o) => Ok(pyo3::types::PyString::new(py, o.as_str()).to_object(py)),
```

### Comparing `cryptography-41.0.0/src/rust/src/x509/common.rs` & `cryptography-41.0.1/src/rust/src/x509/common.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/crl.rs` & `cryptography-41.0.1/src/rust/src/x509/crl.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/csr.rs` & `cryptography-41.0.1/src/rust/src/x509/csr.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/extensions.rs` & `cryptography-41.0.1/src/rust/src/x509/extensions.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/mod.rs` & `cryptography-41.0.1/src/rust/src/x509/mod.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/ocsp.rs` & `cryptography-41.0.1/src/rust/src/x509/ocsp.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/ocsp_req.rs` & `cryptography-41.0.1/src/rust/src/x509/ocsp_req.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/ocsp_resp.rs` & `cryptography-41.0.1/src/rust/src/x509/ocsp_resp.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/sct.rs` & `cryptography-41.0.1/src/rust/src/x509/sct.rs`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/src/rust/src/x509/sign.rs` & `cryptography-41.0.1/src/rust/src/x509/sign.rs`

 * *Files 0% similar despite different names*

```diff
@@ -230,27 +230,27 @@
         }),
         (KeyType::Ed25519 | KeyType::Ed448, _) => Err(pyo3::exceptions::PyValueError::new_err(
             "Algorithm must be None when signing via ed25519 or ed448",
         )),
 
         (KeyType::Ec, HashType::Sha224) => Ok(common::AlgorithmIdentifier {
             oid: asn1::DefinedByMarker::marker(),
-            params: common::AlgorithmParameters::EcDsaWithSha224,
+            params: common::AlgorithmParameters::EcDsaWithSha224(None),
         }),
         (KeyType::Ec, HashType::Sha256) => Ok(common::AlgorithmIdentifier {
             oid: asn1::DefinedByMarker::marker(),
-            params: common::AlgorithmParameters::EcDsaWithSha256,
+            params: common::AlgorithmParameters::EcDsaWithSha256(None),
         }),
         (KeyType::Ec, HashType::Sha384) => Ok(common::AlgorithmIdentifier {
             oid: asn1::DefinedByMarker::marker(),
-            params: common::AlgorithmParameters::EcDsaWithSha384,
+            params: common::AlgorithmParameters::EcDsaWithSha384(None),
         }),
         (KeyType::Ec, HashType::Sha512) => Ok(common::AlgorithmIdentifier {
             oid: asn1::DefinedByMarker::marker(),
-            params: common::AlgorithmParameters::EcDsaWithSha512,
+            params: common::AlgorithmParameters::EcDsaWithSha512(None),
         }),
         (KeyType::Ec, HashType::Sha3_224) => Ok(common::AlgorithmIdentifier {
             oid: asn1::DefinedByMarker::marker(),
             params: common::AlgorithmParameters::EcDsaWithSha3_224,
         }),
         (KeyType::Ec, HashType::Sha3_256) => Ok(common::AlgorithmIdentifier {
             oid: asn1::DefinedByMarker::marker(),
@@ -479,18 +479,18 @@
         | common::AlgorithmParameters::RsaWithSha384(..)
         | common::AlgorithmParameters::RsaWithSha512(..)
         | common::AlgorithmParameters::RsaWithSha3_224(..)
         | common::AlgorithmParameters::RsaWithSha3_256(..)
         | common::AlgorithmParameters::RsaWithSha3_384(..)
         | common::AlgorithmParameters::RsaWithSha3_512(..)
         | common::AlgorithmParameters::RsaPss(..) => Ok(KeyType::Rsa),
-        common::AlgorithmParameters::EcDsaWithSha224
-        | common::AlgorithmParameters::EcDsaWithSha256
-        | common::AlgorithmParameters::EcDsaWithSha384
-        | common::AlgorithmParameters::EcDsaWithSha512
+        common::AlgorithmParameters::EcDsaWithSha224(..)
+        | common::AlgorithmParameters::EcDsaWithSha256(..)
+        | common::AlgorithmParameters::EcDsaWithSha384(..)
+        | common::AlgorithmParameters::EcDsaWithSha512(..)
         | common::AlgorithmParameters::EcDsaWithSha3_224
         | common::AlgorithmParameters::EcDsaWithSha3_256
         | common::AlgorithmParameters::EcDsaWithSha3_384
         | common::AlgorithmParameters::EcDsaWithSha3_512 => Ok(KeyType::Ec),
         common::AlgorithmParameters::Ed25519 => Ok(KeyType::Ed25519),
         common::AlgorithmParameters::Ed448 => Ok(KeyType::Ed448),
         common::AlgorithmParameters::DsaWithSha224
@@ -612,18 +612,18 @@
                     py,
                     "cryptography.hazmat.primitives.asymmetric.padding"
                 ))?
                 .getattr(pyo3::intern!(py, "PKCS1v15"))?
                 .call0()?;
             Ok(pkcs)
         }
-        common::AlgorithmParameters::EcDsaWithSha224
-        | common::AlgorithmParameters::EcDsaWithSha256
-        | common::AlgorithmParameters::EcDsaWithSha384
-        | common::AlgorithmParameters::EcDsaWithSha512
+        common::AlgorithmParameters::EcDsaWithSha224(_)
+        | common::AlgorithmParameters::EcDsaWithSha256(_)
+        | common::AlgorithmParameters::EcDsaWithSha384(_)
+        | common::AlgorithmParameters::EcDsaWithSha512(_)
         | common::AlgorithmParameters::EcDsaWithSha3_224
         | common::AlgorithmParameters::EcDsaWithSha3_256
         | common::AlgorithmParameters::EcDsaWithSha3_384
         | common::AlgorithmParameters::EcDsaWithSha3_512 => {
             let signature_hash_algorithm =
                 identify_signature_hash_algorithm(py, signature_algorithm)?;
 
@@ -678,18 +678,30 @@
                 &common::AlgorithmParameters::RsaWithSha3_384(Some(())),
                 KeyType::Rsa,
             ),
             (
                 &common::AlgorithmParameters::RsaWithSha3_512(Some(())),
                 KeyType::Rsa,
             ),
-            (&common::AlgorithmParameters::EcDsaWithSha224, KeyType::Ec),
-            (&common::AlgorithmParameters::EcDsaWithSha256, KeyType::Ec),
-            (&common::AlgorithmParameters::EcDsaWithSha384, KeyType::Ec),
-            (&common::AlgorithmParameters::EcDsaWithSha512, KeyType::Ec),
+            (
+                &common::AlgorithmParameters::EcDsaWithSha224(None),
+                KeyType::Ec,
+            ),
+            (
+                &common::AlgorithmParameters::EcDsaWithSha256(None),
+                KeyType::Ec,
+            ),
+            (
+                &common::AlgorithmParameters::EcDsaWithSha384(None),
+                KeyType::Ec,
+            ),
+            (
+                &common::AlgorithmParameters::EcDsaWithSha512(None),
+                KeyType::Ec,
+            ),
             (&common::AlgorithmParameters::EcDsaWithSha3_224, KeyType::Ec),
             (&common::AlgorithmParameters::EcDsaWithSha3_256, KeyType::Ec),
             (&common::AlgorithmParameters::EcDsaWithSha3_384, KeyType::Ec),
             (&common::AlgorithmParameters::EcDsaWithSha3_512, KeyType::Ec),
             (&common::AlgorithmParameters::Ed25519, KeyType::Ed25519),
             (&common::AlgorithmParameters::Ed448, KeyType::Ed448),
             (&common::AlgorithmParameters::DsaWithSha224, KeyType::Dsa),
```

### Comparing `cryptography-41.0.0/tests/bench/test_aead.py` & `cryptography-41.0.1/tests/bench/test_aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/bench/test_x509.py` & `cryptography-41.0.1/tests/bench/test_x509.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/conftest.py` & `cryptography-41.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/doubles.py` & `cryptography-41.0.1/tests/doubles.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/backends/test_openssl.py` & `cryptography-41.0.1/tests/hazmat/backends/test_openssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/backends/test_openssl_memleak.py` & `cryptography-41.0.1/tests/hazmat/backends/test_openssl_memleak.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/bindings/test_openssl.py` & `cryptography-41.0.1/tests/hazmat/bindings/test_openssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/fixtures_dh.py` & `cryptography-41.0.1/tests/hazmat/primitives/fixtures_dh.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/fixtures_dsa.py` & `cryptography-41.0.1/tests/hazmat/primitives/fixtures_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/fixtures_ec.py` & `cryptography-41.0.1/tests/hazmat/primitives/fixtures_ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/fixtures_rsa.py` & `cryptography-41.0.1/tests/hazmat/primitives/fixtures_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_3des.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_3des.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_aead.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_aes.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_aes.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_aes_gcm.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_aes_gcm.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_arc4.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_arc4.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_asym_utils.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_asym_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_block.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_block.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_blowfish.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_blowfish.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_camellia.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_camellia.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_cast5.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_cast5.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_chacha20.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_chacha20.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_ciphers.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_cmac.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_concatkdf.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_concatkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_constant_time.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_constant_time.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_dh.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_dh.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_dsa.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_ec.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_ed25519.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_ed25519.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,21 @@
             (
                 serialization.Encoding.DER,
                 serialization.PrivateFormat.PKCS8,
                 serialization.NoEncryption(),
                 None,
                 serialization.load_der_private_key,
             ),
+            (
+                serialization.Encoding.DER,
+                serialization.PrivateFormat.PKCS8,
+                serialization.BestAvailableEncryption(b"\x00"),
+                b"\x00",
+                serialization.load_der_private_key,
+            ),
         ],
     )
     def test_round_trip_private_serialization(
         self, encoding, fmt, encryption, passwd, load_func, backend
     ):
         key = Ed25519PrivateKey.generate()
         serialized = key.private_bytes(encoding, fmt, encryption)
```

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_ed448.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_ed448.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_hash_vectors.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_hash_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_hashes.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_hashes.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_hkdf.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_hkdf_vectors.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_hkdf_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_hmac.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_hmac_vectors.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_hmac_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_idea.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_kbkdf.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_kbkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_keywrap.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_padding.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_padding.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_pbkdf2hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_pkcs12.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_pkcs12.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_pkcs7.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_pkcs7.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_poly1305.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_poly1305.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_rsa.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_scrypt.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_scrypt.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_seed.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_serialization.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_serialization.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_sm4.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_sm4.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_ssh.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_ssh.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_x25519.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_x25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_x448.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_x448.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_x963_vectors.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_x963_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/test_x963kdf.py` & `cryptography-41.0.1/tests/hazmat/primitives/test_x963kdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_hotp.py` & `cryptography-41.0.1/tests/hazmat/primitives/twofactor/test_hotp.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_totp.py` & `cryptography-41.0.1/tests/hazmat/primitives/twofactor/test_totp.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/primitives/utils.py` & `cryptography-41.0.1/tests/hazmat/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/hazmat/test_oid.py` & `cryptography-41.0.1/tests/hazmat/test_oid.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/test_cryptography_utils.py` & `cryptography-41.0.1/tests/test_cryptography_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/test_fernet.py` & `cryptography-41.0.1/tests/test_fernet.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/test_meta.py` & `cryptography-41.0.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/test_rust_utils.py` & `cryptography-41.0.1/tests/test_rust_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/test_utils.py` & `cryptography-41.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/test_warnings.py` & `cryptography-41.0.1/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/utils.py` & `cryptography-41.0.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_aes.py` & `cryptography-41.0.1/tests/wycheproof/test_aes.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_chacha20poly1305.py` & `cryptography-41.0.1/tests/wycheproof/test_chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_cmac.py` & `cryptography-41.0.1/tests/wycheproof/test_cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_dsa.py` & `cryptography-41.0.1/tests/wycheproof/test_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_ecdh.py` & `cryptography-41.0.1/tests/wycheproof/test_ecdh.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_ecdsa.py` & `cryptography-41.0.1/tests/wycheproof/test_ecdsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_eddsa.py` & `cryptography-41.0.1/tests/wycheproof/test_eddsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_hkdf.py` & `cryptography-41.0.1/tests/wycheproof/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_hmac.py` & `cryptography-41.0.1/tests/wycheproof/test_hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_keywrap.py` & `cryptography-41.0.1/tests/wycheproof/test_keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_rsa.py` & `cryptography-41.0.1/tests/wycheproof/test_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_x25519.py` & `cryptography-41.0.1/tests/wycheproof/test_x25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/test_x448.py` & `cryptography-41.0.1/tests/wycheproof/test_x448.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/wycheproof/utils.py` & `cryptography-41.0.1/tests/wycheproof/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/x509/test_name.py` & `cryptography-41.0.1/tests/x509/test_name.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/x509/test_ocsp.py` & `cryptography-41.0.1/tests/x509/test_ocsp.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/x509/test_x509.py` & `cryptography-41.0.1/tests/x509/test_x509.py`

 * *Files 0% similar despite different names*

```diff
@@ -5195,14 +5195,29 @@
         )
         public_key.verify(
             cert.signature,
             cert.tbs_certificate_bytes,
             cert.signature_algorithm_parameters,
         )
 
+    def test_load_ecdsa_cert_null_alg_params(self, backend):
+        """
+        This test verifies that we successfully load certificates with encoded
+        null parameters in the signature AlgorithmIdentifier. This is invalid,
+        but Java 11 (up to at least 11.0.19) generates certificates with this
+        encoding so we need to tolerate it at the moment.
+        """
+        with pytest.warns(utils.DeprecatedIn41):
+            cert = _load_cert(
+                os.path.join("x509", "custom", "ecdsa_null_alg.pem"),
+                x509.load_pem_x509_certificate,
+            )
+            assert isinstance(cert.signature_hash_algorithm, hashes.SHA256)
+            assert isinstance(cert.public_key(), ec.EllipticCurvePublicKey)
+
     def test_load_bitstring_dn(self, backend):
         cert = _load_cert(
             os.path.join("x509", "scottishpower-bitstring-dn.pem"),
             x509.load_pem_x509_certificate,
         )
         assert cert.subject == x509.Name(
             [
```

### Comparing `cryptography-41.0.0/tests/x509/test_x509_crlbuilder.py` & `cryptography-41.0.1/tests/x509/test_x509_crlbuilder.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/x509/test_x509_ext.py` & `cryptography-41.0.1/tests/x509/test_x509_ext.py`

 * *Files identical despite different names*

### Comparing `cryptography-41.0.0/tests/x509/test_x509_revokedcertbuilder.py` & `cryptography-41.0.1/tests/x509/test_x509_revokedcertbuilder.py`

 * *Files identical despite different names*

