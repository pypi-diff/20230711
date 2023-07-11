# Comparing `tmp/sigstore-protobuf-specs-0.1.0.tar.gz` & `tmp/sigstore_protobuf_specs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore-protobuf-specs-0.1.0.tar", last modified: Thu Jan 12 13:36:43 2023, max compression
+gzip compressed data, was "sigstore_protobuf_specs-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore-protobuf-specs-0.1.0.tar` & `sigstore_protobuf_specs-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11358 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/LICENSE
--rw-r--r--   0        0        0      216 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/README.md
--rw-r--r--   0        0        0     1200 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/bundle/__init__.py
--rw-r--r--   0        0        0     3058 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/common/__init__.py
--rw-r--r--   0        0        0     7085 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/rekor/__init__.py
--rw-r--r--   0        0        0     5485 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/trustroot/__init__.py
--rw-r--r--   0        0        0     3969 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/verification/__init__.py
--rw-r--r--   0        0        0     6009 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/google/__init__.py
--rw-r--r--   0        0        0     2081 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/google/api/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/io/__init__.py
--rw-r--r--   0        0        0     1405 2023-01-12 13:36:19.910735 sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/io/intoto/__init__.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 sigstore-protobuf-specs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/LICENSE
+-rw-r--r--   0        0        0      216 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/README.md
+-rw-r--r--   0        0        0     1200 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/bundle/__init__.py
+-rw-r--r--   0        0        0     3438 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/common/__init__.py
+-rw-r--r--   0        0        0     7734 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/rekor/__init__.py
+-rw-r--r--   0        0        0     6228 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/trustroot/__init__.py
+-rw-r--r--   0        0        0     4620 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/verification/__init__.py
+-rw-r--r--   0        0        0     6009 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/google/__init__.py
+-rw-r--r--   0        0        0     2081 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/io/__init__.py
+-rw-r--r--   0        0        0     1417 2023-07-11 20:06:27.948182 sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/io/intoto/__init__.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 sigstore_protobuf_specs-0.2.0/PKG-INFO
```

### Comparing `sigstore-protobuf-specs-0.1.0/LICENSE` & `sigstore_protobuf_specs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore-protobuf-specs-0.1.0/pyproject.toml` & `sigstore_protobuf_specs-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sigstore-protobuf-specs"
-version = "0.1.0"
+version = "0.2.0"
 description = "A library for serializing and deserializing Sigstore messages"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
   { name = "Sigstore Authors", email = "sigstore-dev@googlegroups.com" }
 ]
 classifiers = [
```

### Comparing `sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py` & `sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,30 +43,34 @@
     x509_certificate_chain: "__common_v1__.X509CertificateChain" = (
         betterproto.message_field(2, group="content")
     )
     tlog_entries: List["__rekor_v1__.TransparencyLogEntry"] = betterproto.message_field(
         3
     )
     """
-    This is the inclusion promise and/or proof, where the timestamp is coming
-    from the transparency log.
+    This is the inclusion proof, where the timestamp is coming from the
+    transparency log. Client verification libraries MAY provide an option to
+    support v0.1 bundles for backwards compatibility, which may contain an
+    inclusion promise and not an inclusion proof. In this case, the client MUST
+    validate the promise. Verifiers SHOULD NOT allow v0.1 bundles if they're
+    used in an ecosystem which never produced them.
     """
 
     timestamp_verification_data: "TimestampVerificationData" = (
         betterproto.message_field(4)
     )
     """Timestamp verification data, over the artifact's signature."""
 
 
 @dataclass(eq=False, repr=False)
 class Bundle(betterproto.Message):
     media_type: str = betterproto.string_field(1)
     """
-    MUST be application/vnd.dev.sigstore.bundle+json;version=0.1 when encoded
-    as JSON.
+    MUST be application/vnd.dev.sigstore.bundle+json;version=0.1 or
+    application/vnd.dev.sigstore.bundle+json;version=0.2 when encoded as JSON.
     """
 
     verification_material: "VerificationMaterial" = betterproto.message_field(2)
     """
     When a signer is identified by a X.509 certificate, a verifier MUST verify
     that the signature was computed at the time the certificate was valid as
     described in the Sigstore client spec: "Verification using a Bundle". <http
```

### Comparing `sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py` & `sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -98,16 +98,17 @@
 @dataclass(eq=False, repr=False)
 class LogId(betterproto.Message):
     """LogId captures the identity of a transparency log."""
 
     key_id: bytes = betterproto.bytes_field(1)
     """
     The unique id of the log, represented as the SHA-256 hash of the log's
-    public key, computed over the DER encoding. <https://www.rfc-
-    editor.org/rfc/rfc6962#section-3.2>
+    public key, calculated over the DER encoding of the key represented as
+    SubjectPublicKeyInfo. See https://www.rfc-
+    editor.org/rfc/rfc6962#section-3.2
     """
 
 
 @dataclass(eq=False, repr=False)
 class Rfc3161SignedTimestamp(betterproto.Message):
     """This message holds a RFC 3161 timestamp."""
 
@@ -130,15 +131,15 @@
 
     key_details: "PublicKeyDetails" = betterproto.enum_field(2)
     """Key encoding and signature algorithm to use for this key."""
 
     valid_for: Optional["TimeRange"] = betterproto.message_field(
         3, optional=True, group="_valid_for"
     )
-    """Optional validity period for this key."""
+    """Optional validity period for this key, *inclusive* of the endpoints."""
 
 
 @dataclass(eq=False, repr=False)
 class PublicKeyIdentifier(betterproto.Message):
     """
     PublicKeyIdentifier can be used to identify an (out of band) delivered key,
     to verify a signature.
@@ -195,23 +196,30 @@
 @dataclass(eq=False, repr=False)
 class X509CertificateChain(betterproto.Message):
     """A chain of X.509 certificates."""
 
     certificates: List["X509Certificate"] = betterproto.message_field(1)
     """
     The chain of certificates, with indices 0 to n. The first certificate in
-    the array must be the leaf certificate used for signing. Any intermediate
-    certificates must be stored as offset 1 to n-1, and the root certificate at
-    position n.
+    the array must be the leaf certificate used for signing. Signers MUST NOT
+    include their root CA certificates in their embedded certificate chains,
+    and SHOULD NOT include intermediate CA certificates that appear in
+    independent roots of trust. Verifiers MUST validate the chain carefully to
+    ensure that it chains up to a root CA certificate that they trust,
+    regardless of whether the chain includes additional intermediate/root CA
+    certificates. Verifiers MAY enforce additional constraints, such as
+    requiring that all intermediate CA certificates appear in an independent
+    root of trust. Verifiers SHOULD handle old or non-complying bundles that
+    have additional intermediate/root CA certificates.
     """
 
 
 @dataclass(eq=False, repr=False)
 class TimeRange(betterproto.Message):
     """
-    The time range is half-open and does not include the end timestamp, i.e
-    [start, end). End is optional to be able to capture a period that has
+    The time range is closed and includes both the start and end times, (i.e.,
+    [start, end]). End is optional to be able to capture a period that has
     started but has no known end.
     """
 
     start: datetime = betterproto.message_field(1)
     end: Optional[datetime] = betterproto.message_field(2, optional=True, group="_end")
```

### Comparing `sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py` & `sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     envelope: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class InclusionProof(betterproto.Message):
     """
     InclusionProof is the proof returned from the transparency log. Can be used
-    for on line verification against the log.
+    for offline or online verification against the log.
     """
 
     log_index: int = betterproto.int64_field(1)
     """The index of the entry in the log."""
 
     root_hash: bytes = betterproto.bytes_field(2)
     """
@@ -97,16 +97,15 @@
     TransparencyLogEntry captures all the details required from Rekor to
     reconstruct an entry, given that the payload is provided via other means.
     This type can easily be created from the existing response from Rekor.
     Future iterations could rely on Rekor returning the minimal set of
     attributes (excluding the payload) that are required for verifying the
     inclusion promise. The inclusion promise (called SignedEntryTimestamp in
     the response from Rekor) is similar to a Signed Certificate Timestamp as
-    described here https://www.rfc-editor.org/rfc/rfc9162#name-signed-
-    certificate-timestam.
+    described here https://www.rfc-editor.org/rfc/rfc6962.html#section-3.2.
     """
 
     log_index: int = betterproto.int64_field(1)
     """The index of the entry in the log."""
 
     log_id: "__common_v1__.LogId" = betterproto.message_field(2)
     """The unique identifier of the log."""
@@ -117,23 +116,35 @@
     values are required to construct the entry during verification.
     """
 
     integrated_time: int = betterproto.int64_field(4)
     """The UNIX timestamp from the log when the entry was persisted."""
 
     inclusion_promise: "InclusionPromise" = betterproto.message_field(5)
-    """The inclusion promise/signed entry timestamp from the log."""
+    """
+    The inclusion promise/signed entry timestamp from the log. Required for
+    v0.1 bundles, and MUST be verified. Optional for >= v0.2 bundles, and
+    SHOULD be verified when present.
+    """
 
     inclusion_proof: "InclusionProof" = betterproto.message_field(6)
     """
-    The inclusion proof can be used for online verification that the entry was
-    appended to the log, and that the log has not been altered.
+    The inclusion proof can be used for offline or online verification that the
+    entry was appended to the log, and that the log has not been altered.
     """
 
     canonicalized_body: bytes = betterproto.bytes_field(7)
     """
-    The canonicalized Rekor entry body, used for SET verification. This is the
-    same as the body returned by Rekor. It's included here for cases where the
-    client cannot deterministically reconstruct the bundle from the other
-    fields. Clients MUST verify that the signature referenced in the
-    canonicalized_body matches the signature provided in the bundle content.
+    Optional. The canonicalized transparency log entry, used to reconstruct the
+    Signed Entry Timestamp (SET) during verification. The contents of this
+    field are the same as the `body` field in a Rekor response, meaning that it
+    does **not** include the "full" canonicalized form (of log index, ID, etc.)
+    which are exposed as separate fields. The verifier is responsible for
+    combining the `canonicalized_body`, `log_index`, `log_id`, and
+    `integrated_time` into the payload that the SET's signature is generated
+    over. This field is intended to be used in cases where the SET cannot be
+    produced determinisitically (e.g. inconsistent JSON field ordering,
+    differing whitespace, etc). If set, clients MUST verify that the signature
+    referenced in the `canonicalized_body` matches the signature provided in
+    the `Bundle.content`. If not set, clients are responsible for constructing
+    an equivalent payload from other sources to verify the signature.
     """
```

### Comparing `sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py` & `sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 
 @dataclass(eq=False, repr=False)
 class TransparencyLogInstance(betterproto.Message):
     """
     TransparencyLogInstance describes the immutable parameters from a
     transparency log. See https://www.rfc-editor.org/rfc/rfc9162.html#name-log-
-    parameters for more details. The incluced parameters are the minimal set
-    required to identify a log, and verify an inclusion promise.
+    parameters for more details. The included parameters are the minimal set
+    required to identify a log, and verify an inclusion proof/promise.
     """
 
     base_url: str = betterproto.string_field(1)
     """The base URL at which can be used to URLs for the client."""
 
     hash_algorithm: "__common_v1__.HashAlgorithm" = betterproto.enum_field(2)
     """The hash algorithm used for the Merkle Tree."""
@@ -53,41 +53,50 @@
     cert_chain: "__common_v1__.X509CertificateChain" = betterproto.message_field(3)
     """The certificate chain for this CA."""
 
     valid_for: "__common_v1__.TimeRange" = betterproto.message_field(4)
     """
     The time the *entire* chain was valid. This is at max the longest interval
     when *all* certificates in the chain were valid, but it MAY be shorter.
+    Clients MUST check timestamps against *both* the `valid_for` time range
+    *and* the entire certificate chain. The TimeRange should be considered
+    valid *inclusive* of the endpoints.
     """
 
 
 @dataclass(eq=False, repr=False)
 class TrustedRoot(betterproto.Message):
     """
     TrustedRoot describes the client's complete set of trusted entities. How
     the TrustedRoot is populated is not specified, but can be a combination of
     many sources such as TUF repositories, files on disk etc. The TrustedRoot
     is not meant to be used for any artifact verification, only to capture the
     complete/global set of trusted verification materials. When verifying an
     artifact, based on the artifact and policies, a selection of
     keys/authorities are expected to be extracted and provided to the
-    verification function. This way the set of keys/authorities kan be kept to
+    verification function. This way the set of keys/authorities can be kept to
     a minimal set by the policy to gain better control over what signatures
-    that are allowed.
+    that are allowed. The embedded transparency logs, CT logs, CAs and TSAs
+    MUST include any previously used instance -- otherwise signatures made in
+    the past cannot be verified. The currently used instances MUST NOT have
+    their 'end' timestamp set in their 'valid_for' attribute for easy
+    identification. All the listed instances SHOULD be sorted by the
+    'valid_for' in ascending order, that is, the oldest instance first and the
+    current instance last.
     """
 
     media_type: str = betterproto.string_field(1)
     """MUST be application/vnd.dev.sigstore.trustedroot+json;version=0.1"""
 
     tlogs: List["TransparencyLogInstance"] = betterproto.message_field(2)
     """A set of trusted Rekor servers."""
 
     certificate_authorities: List["CertificateAuthority"] = betterproto.message_field(3)
     """
-    A set of trusted certificate authorites (e.g Fulcio), and any intermediate
+    A set of trusted certificate authorities (e.g Fulcio), and any intermediate
     certificates they provide. If a CA is issuing multiple intermediate
     certificate, each combination shall be represented as separate chain. I.e,
     a single root cert may appear in multiple chains but with different
     intermediate and/or leaf certificates. The certificates are intended to be
     used for verifying artifact signatures.
     """
```

### Comparing `sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py` & `sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/google/api/__init__.py` & `sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-protobuf-specs-0.1.0/sigstore_protobuf_specs/io/intoto/__init__.py` & `sigstore_protobuf_specs-0.2.0/sigstore_protobuf_specs/io/intoto/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     """
 
     payload_type: str = betterproto.string_field(2)
     """String unambiguously identifying how to interpret payload. REQUIRED."""
 
     signatures: List["Signature"] = betterproto.message_field(3)
     """
-    Signature over:     PAE(type, body) Where PAE is defined as: PAE(type,
-    body) = "DSSEv1" + SP + LEN(type) + SP + type + SP + LEN(body) + SP + body
-    +               = concatenation SP              = ASCII space [0x20]
-    "DSSEv1"        = ASCII [0x44, 0x53, 0x53, 0x45, 0x76, 0x31] LEN(s)
+    Signature over:     PAE(type, payload) Where PAE is defined as: PAE(type,
+    payload) = "DSSEv1" + SP + LEN(type) + SP + type + SP + LEN(payload) + SP +
+    payload +               = concatenation SP              = ASCII space
+    [0x20] "DSSEv1"        = ASCII [0x44, 0x53, 0x53, 0x45, 0x76, 0x31] LEN(s)
     = ASCII decimal encoding of the byte length of s, with no leading zeros
     REQUIRED (length >= 1).
     """
 
 
 @dataclass(eq=False, repr=False)
 class Signature(betterproto.Message):
```

### Comparing `sigstore-protobuf-specs-0.1.0/PKG-INFO` & `sigstore_protobuf_specs-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore-protobuf-specs
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library for serializing and deserializing Sigstore messages
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

