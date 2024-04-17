# Comparing `tmp/pycvc-1.4.0.tar.gz` & `tmp/pycvc-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycvc-1.4.0.tar", last modified: Fri Aug 25 13:39:38 2023, max compression
+gzip compressed data, was "pycvc-1.5.0.tar", last modified: Wed Apr 17 12:23:13 2024, max compression
```

## Comparing `pycvc-1.4.0.tar` & `pycvc-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 13:39:38.807287 pycvc-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (999)     8774 2023-08-25 13:39:38.807287 pycvc-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     7576 2023-08-25 13:39:25.000000 pycvc-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 13:39:38.803287 pycvc-1.4.0/cvc/
--rw-r--r--   0 runner    (1001) docker     (999)       34 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      770 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)     3507 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/asn1.py
--rw-r--r--   0 runner    (1001) docker     (999)    10505 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/certificates.py
--rw-r--r--   0 runner    (1001) docker     (999)    12817 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/ec_curves.py
--rw-r--r--   0 runner    (1001) docker     (999)     8040 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/oid.py
--rw-r--r--   0 runner    (1001) docker     (999)     2716 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 13:39:38.807287 pycvc-1.4.0/cvc/tools/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (999)    13606 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/tools/cvc_create.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     4979 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/tools/cvc_print.py
--rw-r--r--   0 runner    (1001) docker     (999)     2702 2023-08-25 13:39:25.000000 pycvc-1.4.0/cvc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 13:39:38.807287 pycvc-1.4.0/pycvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     8774 2023-08-25 13:39:38.000000 pycvc-1.4.0/pycvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      384 2023-08-25 13:39:38.000000 pycvc-1.4.0/pycvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-25 13:39:38.000000 pycvc-1.4.0/pycvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       92 2023-08-25 13:39:38.000000 pycvc-1.4.0/pycvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-08-25 13:39:38.000000 pycvc-1.4.0/pycvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-08-25 13:39:38.000000 pycvc-1.4.0/pycvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-25 13:39:38.807287 pycvc-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     3030 2023-08-25 13:39:25.000000 pycvc-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:23:13.522358 pycvc-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-17 12:23:13.522358 pycvc-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-17 12:23:05.000000 pycvc-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:23:13.518358 pycvc-1.5.0/cvc/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/asn1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12975 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/ec_curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/oid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:23:13.518358 pycvc-1.5.0/cvc/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13604 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/tools/cvc_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/tools/cvc_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-17 12:23:05.000000 pycvc-1.5.0/cvc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:23:13.522358 pycvc-1.5.0/pycvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-17 12:23:13.000000 pycvc-1.5.0/pycvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 12:23:13.000000 pycvc-1.5.0/pycvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:23:13.000000 pycvc-1.5.0/pycvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 12:23:13.000000 pycvc-1.5.0/pycvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 12:23:13.000000 pycvc-1.5.0/pycvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 12:23:13.000000 pycvc-1.5.0/pycvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:23:13.522358 pycvc-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-17 12:23:05.000000 pycvc-1.5.0/setup.py
```

### Comparing `pycvc-1.4.0/PKG-INFO` & `pycvc-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycvc
-Version: 1.4.0
+Version: 1.5.0
 Summary: Card Verifiable Certificate tools
 Home-page: https://github.com/polhenarejos/pycvc
 Author: Pol Henarejos
 Author-email: pol.henarejos@cttc.es
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -22,14 +22,16 @@
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
+Requires-Dist: setuptools
+Requires-Dist: cryptography>=3.3
 
 # pycvc
 Card Verifiable Certificates (CVC) tools for Python
 
 ## Introduction
 
 Card Verifiable Certificates are an specification of storing electronic certificates, signed by RSA or Elliptic Curves algorithms.
@@ -53,15 +55,15 @@
 pycvc can be used by importing the package or calling the command line tools `cvc-create`, for CVC generation, and `cvc-print`, for displaying CVC information and verification.
 
 For more information, execute `cvc-create` or `cvc-print` with `--help` flag.
 
 **Supported algorithms**
 - RSA
 - ECDSA
-- EDDSA
+- EdDSA
 
 **Supported curves**
 - secp192r1 (prime192v1)
 - secp224r1
 - secp256r1 (prime256v1)
 - secp384r1
 - secp521r1
@@ -80,14 +82,15 @@
 - ECDSA_SHA_512
 - RSA_v1_5_SHA_1
 - RSA_v1_5_SHA_256
 - RSA_v1_5_SHA_512
 - RSA_PSS_SHA_1
 - RSA_PSS_SHA_256
 - RSA_PSS_SHA_512
+- EDDSA
 
 Here some examples.
 
 ### Create a PKI with ECDSA
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
```

### Comparing `pycvc-1.4.0/README.md` & `pycvc-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 pycvc can be used by importing the package or calling the command line tools `cvc-create`, for CVC generation, and `cvc-print`, for displaying CVC information and verification.
 
 For more information, execute `cvc-create` or `cvc-print` with `--help` flag.
 
 **Supported algorithms**
 - RSA
 - ECDSA
-- EDDSA
+- EdDSA
 
 **Supported curves**
 - secp192r1 (prime192v1)
 - secp224r1
 - secp256r1 (prime256v1)
 - secp384r1
 - secp521r1
@@ -51,14 +51,15 @@
 - ECDSA_SHA_512
 - RSA_v1_5_SHA_1
 - RSA_v1_5_SHA_256
 - RSA_v1_5_SHA_512
 - RSA_PSS_SHA_1
 - RSA_PSS_SHA_256
 - RSA_PSS_SHA_512
+- EDDSA
 
 Here some examples.
 
 ### Create a PKI with ECDSA
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
```

### Comparing `pycvc-1.4.0/cvc/_version.py` & `pycvc-1.5.0/cvc/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
  * General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program. If not, see <http://www.gnu.org/licenses/>.
  */
 """
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
```

### Comparing `pycvc-1.4.0/cvc/asn1.py` & `pycvc-1.5.0/cvc/asn1.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.4.0/cvc/certificates.py` & `pycvc-1.5.0/cvc/certificates.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 from cryptography.hazmat.primitives.asymmetric import ec, rsa, utils, x25519, x448, ed25519, ed448
 from cryptography.exceptions import InvalidSignature
 import datetime
 from cvc.utils import to_bytes, bcd, get_hash_padding, scheme_rsa
 from cvc.ec_curves import EcCurve
 from cvc.asn1 import ASN1
-import os
+from cvc.terminal import Type
+import os, math
 
 class CVC:
     __data=None
     def __init__(self):
         self.__a = ASN1()
 
     def decode(self, data):
@@ -102,15 +103,20 @@
             Y = pubkey.public_bytes(Encoding.Raw, PublicFormat.Raw)
             pubctx = {1: dom.P, 2: dom.O, 3: dom.G, 4: Y}
         self.__a = self.__a.add_object(0x7f49, scheme, pubctx)
         return self
 
     def role(self, role=None):
         if (self.__data != None):
-            return self.body().find(0x7f4c)
+            d = self.body().find(0x7f4c)
+            if (d):
+                o = d.oid()
+                chat = self.body().find(0x7f4c).find(0x53).data()
+                return Type.from_bytes(o, chat)
+            return None
         if (role != None):
             self.__a = self.__a.add_tag(0x7f4c, ASN1().add_oid(role.OID).add_tag(0x53, role.to_bytes()).encode())
         return self
 
     def valid(self, days=None, since=None):
         if (self.__data != None):
             return self.body().find(0x5f25).data()
@@ -133,15 +139,16 @@
             return self.req().find(0x5f37).data()
 
     def sign(self, key, scheme):
         h,p = get_hash_padding(scheme)
         if (isinstance(key, ec.EllipticCurvePrivateKey)):
             signature = key.sign(self.__a.encode(), ec.ECDSA(h))
             r,s = utils.decode_dss_signature(signature)
-            signature = to_bytes(r) + to_bytes(s)
+            n = math.ceil(key.curve.key_size / 8)
+            signature = r.to_bytes(n, 'big') + s.to_bytes(n, 'big')
         elif (isinstance(key, rsa.RSAPrivateKey)):
             signature = key.sign(self.__a.encode(), p, h)
         elif (isinstance(key, (ed25519.Ed25519PrivateKey, ed448.Ed448PrivateKey))):
             signature = key.sign(self.__a.encode())
         self.__a = self.__a.add_tag(0x5f37, bytearray(signature))
         return self
 
@@ -208,35 +215,36 @@
                     Q = ASN1().decode(puk).find(0x84).data()
                     pubkey = curve.from_public_bytes(bytes(Q))
                     pubkey.verify(bytes(signature), bytes(body))
                 elif (curve):
                     Q = ASN1().decode(puk).find(0x86).data()
                     if (Q):
                         pubkey = ec.EllipticCurvePublicKey.from_encoded_point(curve, bytes(Q))
-                        pubkey.verify(utils.encode_dss_signature(int.from_bytes(signature[:len(signature)//2],'big'), int.from_bytes(signature[len(signature)//2:],'big')), body, ec.ECDSA(h))
+                        n = math.ceil(pubkey.curve.key_size / 8)
+                        pubkey.verify(utils.encode_dss_signature(int.from_bytes(signature[:n],'big'), int.from_bytes(signature[n:],'big')), body, ec.ECDSA(h))
                 else:
                     return False
         except InvalidSignature:
             return False
         return True
 
     def find_domain(self, cert_dir='', outer=False):
         adata = self.encode()
         try:
             P = CVC().decode(adata).pubkey().find(0x81) if outer is False else None
             if (P):
-                return EcCurve.to_crypto(EcCurve.from_P(P.data()))
+                return EcCurve.from_P(P.data()).to_crypto()
             depth = 10
             while (P == None and depth > 0):
                 car = CVC().decode(adata).outer_car()
                 if (not car or outer is False):
                     car = CVC().decode(adata).car()
                 chr = CVC().decode(adata).chr()
                 with open(os.path.join(cert_dir,bytes(car)), 'rb') as f:
                     adata = f.read()
                     P = CVC().decode(adata).pubkey().find(0x81)
                 if (P):
-                    return EcCurve.to_crypto(EcCurve.from_P(P.data()))
+                    return EcCurve.from_P(P.data()).to_crypto()
                 depth -= 1
         except FileNotFoundError:
             print(f'[Warning: File {car.decode()} not found]')
-        return None
+        return None
```

### Comparing `pycvc-1.4.0/cvc/ec_curves.py` & `pycvc-1.5.0/cvc/ec_curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,31 +28,38 @@
     G = None
     O = None
     F = None
 
     def from_name(name):
         for e in EcCurve.__subclasses__():
             if e.__name__.lower() == name.lower():
-                return e
+                return e()
         return UnsupportedCurve
 
-    def to_crypto(curve):
-        if (curve.__name__ == 'Curve25519'):
+    def __to_crypto(name):
+        name = name.lower()
+        if (name == 'curve25519'):
             return ed25519.Ed25519PublicKey
-        elif (curve.__name__ == 'Curve448'):
+        elif (name == 'curve448'):
             return ed448.Ed448PublicKey
         for e in ec.EllipticCurve.__subclasses__():
-            if (e.__name__.lower() == curve.__name__.lower()):
+            if (e.__name__.lower() == name):
                 return e()
         return UnsupportedCurve
 
+    def to_crypto(curve):
+        return EcCurve.__to_crypto(curve.__name__)
+
+    def to_crypto(self):
+        return EcCurve.__to_crypto(self.__class__.__name__)
+
     def from_P(P):
         for e in EcCurve.__subclasses__():
             if e.P == P:
-                return e
+                return e()
         return UnsupportedCurve
 
 class UnsupportedCurve(EcCurve):
     """Not supported"""
 
 class SECP192R1(EcCurve):
     P = bytearray(unhexlify("FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEFFFFFFFFFFFFFFFF"))
@@ -90,15 +97,14 @@
     P = bytearray(unhexlify("01FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF"))
     A = bytearray(unhexlify("01FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFC"))
     B = bytearray(unhexlify("0051953EB9618E1C9A1F929A21A0B68540EEA2DA725B99B315F3B8B489918EF109E156193951EC7E937B1652C0BD3BB1BF073573DF883D2C34F1EF451FD46B503F00"))
     G = bytearray(unhexlify("0400C6858E06B70404E9CD9E3ECB662395B4429C648139053FB521F828AF606B4D3DBAA14B5E77EFE75928FE1DC127A2FFA8DE3348B3C1856A429BF97E7E31C2E5BD66011839296A789A3BC0045C8A5FB42C7D1BD998F54449579B446817AFBD17273E662C97EE72995EF42640C550B9013FAD0761353C7086A272C24088BE94769FD16650"))
     O = bytearray(unhexlify("01FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFA51868783BF2F966B7FCC0148F709A5D03BB5C9B8899C47AEBB6FB71E91386409"))
     F = bytearray(unhexlify("01"))
 
-
 class BrainpoolP192R1(EcCurve):
     P = bytearray(unhexlify("C302F41D932A36CDA7A3463093D18DB78FCE476DE1A86297"))
     A = bytearray(unhexlify("6A91174076B1E0E19C39C031FE8685C1CAE040E5C69A28EF"))
     B = bytearray(unhexlify("469A28EF7C28CCA3DC721D044F4496BCCA7EF4146FBF25C9"))
     G = bytearray(unhexlify("04C0A0647EAAB6A48753B033C56CB0F0900A2F5C4853375FD614B690866ABD5BB88B5F4828C1490002E6773FA2FA299B8F"))
     O = bytearray(unhexlify("C302F41D932A36CDA7A3462F9E9E916B5BE8F1029AC4ACC1"))
     F = bytearray(unhexlify("01"))
```

### Comparing `pycvc-1.4.0/cvc/oid.py` & `pycvc-1.5.0/cvc/oid.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.4.0/cvc/terminal.py` & `pycvc-1.5.0/cvc/terminal.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,51 +25,76 @@
     CVCA = 3
     DV_domestic = 2
     DV_foreign = 1
     Terminal = 0
 
     __chat = 0
 
-    def __init__(self, role):
+    def __init__(self, role, _args, kwargs):
         self.role = role
+        for attr in _args:
+            setattr(self, attr, kwargs.get(attr, 0))
 
     def to_bytes(self):
-        x = 0
         total = len(self._args)
-        for ix, attr in enumerate(self._args):
-            x = x + 2**(total-ix-1) * getattr(self, attr, 0)
+        x = self.fields()
         x = x + self.role * 2**(total)
         x |= self.__chat
         return x.to_bytes((total + 7) // 8, 'big')
 
     def chat(self, chat):
         if (chat):
             if (isinstance(chat, str)):
                 chat = int(chat, 2)
             self.__chat = chat
 
+    def from_bytes(o, chat):
+        for s in Type.__subclasses__():
+            if (s.OID == o):
+                nargs = len(s._args)
+                chat = int.from_bytes(chat, 'big')
+                kwargs = {attr: (chat >> (nargs - ix - 1)) & 1 for ix, attr in enumerate(s._args)}
+                return s(chat >> nargs, **kwargs)
+        raise Exception('Unknown type')
+
+    def fields_str(self):
+        fields = [bit for ix, bit in enumerate(self._args) if getattr(self, bit, 0) == 1]
+        return ", ".join(fields)
+
+    def fields(self):
+        nargs = len(self._args)
+        x = 0
+        for ix, attr in enumerate(self._args):
+            x = x + 2**(nargs-ix-1) * getattr(self, attr, 0)
+        return x
+
+    def role_str(self):
+        if (self.role == Type.CVCA):
+            return 'CA'
+        elif (self.role == Type.DV_domestic):
+            return 'DV domestic'
+        elif (self.role == Type.DV_foreign):
+            return 'DV foreign'
+        elif (self.role == Type.Terminal):
+            return 'Terminal'
+        return 'Unknown type'
+
 class TypeIS(Type):
     OID = oid.ID_IS
     name = 'TypeIS'
     _args = ('rfu5', 'rfu4', 'rfu3', 'rfu2', 'read_iris', 'read_fingerprint')
     def __init__(self, role, **kwargs):
-        for attr in self._args:
-            setattr(self, attr, kwargs.get(attr, 0))
-        super().__init__(role)
+        super().__init__(role, self._args, kwargs)
 
 class TypeAT(Type):
     OID = oid.ID_AT
     name = 'TypeAT'
     _args = ('write_dg17', 'write_dg18', 'write_dg19', 'write_dg20', 'write_dg21', 'write_dg22', 'rfu31', 'psa', 'read_dg22', 'read_dg21', 'read_dg20', 'read_dg19', 'read_dg18', 'read_dg17', 'read_dg16', 'read_dg15', 'read_dg14', 'read_dg13', 'read_dg12', 'read_dg11', 'read_dg10', 'read_dg9', 'read_dg8', 'read_dg7', 'read_dg6', 'read_dg5', 'read_dg4', 'read_dg3', 'read_dg2', 'read_dg1', 'install_qual_cert', 'install_cert', 'pin_management', 'can_allowed', 'privileged', 'rid', 'verify_community', 'verify_age')
     def __init__(self, role, **kwargs):
-        for attr in self._args:
-            setattr(self, attr, kwargs.get(attr, 0))
-        super().__init__(role)
+        super().__init__(role, self._args, kwargs)
 
 class TypeST(Type):
     OID = oid.ID_ST
     name = 'TypeST'
     _args = ('rfu5', 'rfu4', 'rfu3', 'rfu2', 'gen_qual_sig', 'gen_sig')
     def __init__(self, role, **kwargs):
-        for attr in self._args:
-            setattr(self, attr, kwargs.get(attr, 0))
-        super().__init__(role)
+        super().__init__(role, self._args, kwargs)
```

### Comparing `pycvc-1.4.0/cvc/tools/cvc_create.py` & `pycvc-1.5.0/cvc/tools/cvc_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,17 @@
     parser.add_argument('--read-dg18', help='Allow reading DG 18  (Community ID)', action='store_true')
     parser.add_argument('--read-dg19', help='Allow reading DG 19  (Residence Permit I)', action='store_true')
     parser.add_argument('--read-dg20', help='Allow reading DG 20  (Residence Permit II)', action='store_true')
     parser.add_argument('--read-dg21', help='Allow reading DG 21  (Phone Number)', action='store_true')
     parser.add_argument('--read-dg22', help='Allow reading DG 22  (Email Address)', action='store_true')
     parser.add_argument('--install-qual-cert', help='Allow installing qualified certificate', action='store_true')
     parser.add_argument('--install-cert', help='Allow installing certificate', action='store_true')
-    parser.add_argument('--pin-management ', help='Allow PIN management', action='store_true')
+    parser.add_argument('--pin-management', help='Allow PIN management', action='store_true')
     parser.add_argument('--can-allowed', help='CAN allowed', action='store_true')
-    parser.add_argument('--privileged ', help='Privileged terminal', action='store_true')
+    parser.add_argument('--privileged', help='Privileged terminal', action='store_true')
     parser.add_argument('--rid', help='Allow restricted identification', action='store_true')
     parser.add_argument('--verify-community', help='Allow community ID verification', action='store_true')
     parser.add_argument('--verify-age', help='Allow age verification', action='store_true')
 
     parser.add_argument('--rfu5', help='Allow RFU bit 5', action='store_true')
     parser.add_argument('--rfu4', help='Allow RFU bit 4', action='store_true')
     parser.add_argument('--rfu3', help='Allow RFU bit 3', action='store_true')
@@ -125,15 +125,15 @@
 
 def get_role(r):
     if (r == 'cvca'):
         return Type.CVCA
     elif (r== 'dv_domestic'):
         return Type.DV_domestic
     elif (r == 'dv_foreign'):
-        return Type.dv_foreign
+        return Type.DV_foreign
     elif (r == 'terminal'):
         return Type.Terminal
     return None
 
 def get_type(t, role, args):
     if (t == 'at'):
         typ = TypeAT(role)
```

### Comparing `pycvc-1.4.0/cvc/tools/cvc_print.py` & `pycvc-1.5.0/cvc/tools/cvc_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 """
 
 import argparse, logging, sys
 from cvc.certificates import CVC
 from binascii import hexlify
 from cvc.utils import scheme_rsa, scheme_eddsa
 from cvc.oid import oid2scheme
+from cvc.terminal import Type
 from cvc import __version__, oid
 from datetime import date
 import os
 
 logger = logging.getLogger(__name__)
 cert_dir = b''
 
@@ -69,25 +70,21 @@
         print(f'    Modulus: {hexlify(CVC().decode(cdata).pubkey().find(0x81).data()).decode()}')
         print(f'    Exponent: {hexlify(CVC().decode(cdata).pubkey().find(0x82).data()).decode()}')
     elif (scheme_eddsa(puboid)):
         print(f'    Public Point: {hexlify(CVC().decode(cdata).pubkey().find(0x84).data()).decode()}')
     else:
         print(f'    Public Point: {hexlify(CVC().decode(cdata).pubkey().find(0x86).data()).decode()}')
     print(f'  CHR: {chr.decode()}')
-    role = CVC().decode(cdata).role()
-    if (role):
-        print('  CHAT:')
-        o = role.oid()
-        if (o == oid.ID_IS):
-            print('    Role:  TypeIS')
-        elif (o == oid.ID_AT):
-            print('    Role:  TypeAT')
-        elif (o == oid.ID_ST):
-            print('    Role:  TypeST')
-        print(f'    Bytes: {hexlify(CVC().decode(cdata).role().find(0x53).data()).decode()}')
+    typ = CVC().decode(cdata).role()
+    if (typ):
+        print(f'  CHAT: {typ.name}')
+        print(f'    Role:  {typ.role_str()}')
+        if (typ.fields() > 0):
+            print(f'    Fields: {typ.fields_str()}')
+        print(f'    Bytes: {hexlify(typ.to_bytes()).decode()}')
         print(f'  Since:   {bcd2date(CVC().decode(cdata).valid()).strftime("%Y-%m-%d")}')
         print(f'  Expires: {bcd2date(CVC().decode(cdata).expires()).strftime("%Y-%m-%d")}')
     isreq = CVC().decode(cdata).is_req()
     if (CVC().decode(cdata).verify(cert_dir=cert_dir, dica=cdata if isreq else None)):
         print('Inner signature is VALID')
         ret = True
     else:
```

### Comparing `pycvc-1.4.0/cvc/utils.py` & `pycvc-1.5.0/cvc/utils.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.4.0/pycvc.egg-info/PKG-INFO` & `pycvc-1.5.0/pycvc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycvc
-Version: 1.4.0
+Version: 1.5.0
 Summary: Card Verifiable Certificate tools
 Home-page: https://github.com/polhenarejos/pycvc
 Author: Pol Henarejos
 Author-email: pol.henarejos@cttc.es
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -22,14 +22,16 @@
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
+Requires-Dist: setuptools
+Requires-Dist: cryptography>=3.3
 
 # pycvc
 Card Verifiable Certificates (CVC) tools for Python
 
 ## Introduction
 
 Card Verifiable Certificates are an specification of storing electronic certificates, signed by RSA or Elliptic Curves algorithms.
@@ -53,15 +55,15 @@
 pycvc can be used by importing the package or calling the command line tools `cvc-create`, for CVC generation, and `cvc-print`, for displaying CVC information and verification.
 
 For more information, execute `cvc-create` or `cvc-print` with `--help` flag.
 
 **Supported algorithms**
 - RSA
 - ECDSA
-- EDDSA
+- EdDSA
 
 **Supported curves**
 - secp192r1 (prime192v1)
 - secp224r1
 - secp256r1 (prime256v1)
 - secp384r1
 - secp521r1
@@ -80,14 +82,15 @@
 - ECDSA_SHA_512
 - RSA_v1_5_SHA_1
 - RSA_v1_5_SHA_256
 - RSA_v1_5_SHA_512
 - RSA_PSS_SHA_1
 - RSA_PSS_SHA_256
 - RSA_PSS_SHA_512
+- EDDSA
 
 Here some examples.
 
 ### Create a PKI with ECDSA
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
```

### Comparing `pycvc-1.4.0/setup.py` & `pycvc-1.5.0/setup.py`

 * *Files identical despite different names*

