# Comparing `tmp/moonstreamdb-0.4.1.tar.gz` & `tmp/moonstreamdb-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-0.4.1.tar", last modified: Mon Apr 15 11:07:53 2024, max compression
+gzip compressed data, was "moonstreamdb-0.4.2.tar", last modified: Wed Apr 17 12:59:52 2024, max compression
```

## Comparing `moonstreamdb-0.4.1.tar` & `moonstreamdb-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/moonstreamdb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    61400 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/moonstreamdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/moonstreamdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:07:43.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 11:07:53.000000 moonstreamdb-0.4.1/moonstreamdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:07:53.460712 moonstreamdb-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-15 11:07:36.000000 moonstreamdb-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/moonstreamdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65038 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/moonstreamdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 12:59:52.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:59:39.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/setup.py
```

### Comparing `moonstreamdb-0.4.1/PKG-INFO` & `moonstreamdb-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.4.1
+Version: 0.4.2
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.4.1/README.md` & `moonstreamdb-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.1/moonstreamdb/blockchain.py` & `moonstreamdb-0.4.2/moonstreamdb/blockchain.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     EthereumTransaction,
     MumbaiBlock,
     MumbaiLabel,
     MumbaiTransaction,
     PolygonBlock,
     PolygonLabel,
     PolygonTransaction,
+    ProofOfPlayApexBlock,
+    ProofOfPlayApexLabel,
+    ProofOfPlayApexTransaction,
     WyrmBlock,
     WyrmLabel,
     WyrmTransaction,
     XaiBlock,
     XaiLabel,
     XaiSepoliaBlock,
     XaiSepoliaLabel,
@@ -70,14 +73,15 @@
     ARBITRUM_SEPOLIA = "arbitrum_sepolia"
     XAI = "xai"
     XAI_SEPOLIA = "xai_sepolia"
     AVALANCHE = "avalanche"
     AVALANCHE_FUJI = "avalanche_fuji"
     BLAST = "blast"
     BLAST_SEPOLIA = "blast_sepolia"
+    PROOFOFPLAY_APEX = "proofofplay_apex"
 
 
 def get_block_model(
     blockchain_type: AvailableBlockchainType,
 ) -> Type[
     Union[
         EthereumBlock,
@@ -93,14 +97,15 @@
         ArbitrumSepoliaBlock,
         XaiBlock,
         XaiSepoliaBlock,
         AvalancheBlock,
         AvalancheFujiBlock,
         BlastBlock,
         BlastSepoliaBlock,
+        ProofOfPlayApexBlock,
     ]
 ]:
     """
     Depends on provided blockchain type set proper blocks model.
     """
     block_model: Type[
         Union[
@@ -117,14 +122,15 @@
             ArbitrumSepoliaBlock,
             XaiBlock,
             XaiSepoliaBlock,
             AvalancheBlock,
             AvalancheFujiBlock,
             BlastBlock,
             BlastSepoliaBlock,
+            ProofOfPlayApexBlock,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         block_model = EthereumBlock
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         block_model = PolygonBlock
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
@@ -153,14 +159,16 @@
         block_model = AvalancheBlock
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         block_model = AvalancheFujiBlock
     elif blockchain_type == AvailableBlockchainType.BLAST:
         block_model = BlastBlock
     elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
         block_model = BlastSepoliaBlock
+    elif blockchain_type == AvailableBlockchainType.PROOFOFPLAY_APEX:
+        block_model = ProofOfPlayApexBlock
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return block_model
 
 
 def get_label_model(
@@ -180,14 +188,15 @@
         ArbitrumSepoliaLabel,
         XaiLabel,
         XaiSepoliaLabel,
         AvalancheLabel,
         AvalancheFujiLabel,
         BlastLabel,
         BlastSepoliaLabel,
+        ProofOfPlayApexLabel,
     ]
 ]:
     """
     Depends on provided blockchain type set proper block label model.
     """
     label_model: Type[
         Union[
@@ -204,14 +213,15 @@
             ArbitrumSepoliaLabel,
             XaiLabel,
             XaiSepoliaLabel,
             AvalancheLabel,
             AvalancheFujiLabel,
             BlastLabel,
             BlastSepoliaLabel,
+            ProofOfPlayApexLabel,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         label_model = EthereumLabel
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         label_model = PolygonLabel
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
@@ -240,14 +250,16 @@
         label_model = AvalancheLabel
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         label_model = AvalancheFujiLabel
     elif blockchain_type == AvailableBlockchainType.BLAST:
         label_model = BlastLabel
     elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
         label_model = BlastSepoliaLabel
+    elif blockchain_type == AvailableBlockchainType.PROOFOFPLAY_APEX:
+        label_model = ProofOfPlayApexLabel
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return label_model
 
 
 def get_transaction_model(
@@ -267,14 +279,15 @@
         ArbitrumSepoliaTransaction,
         XaiTransaction,
         XaiSepoliaTransaction,
         AvalancheTransaction,
         AvalancheFujiTransaction,
         BlastTransaction,
         BlastSepoliaTransaction,
+        ProofOfPlayApexTransaction,
     ]
 ]:
     """
     Depends on provided blockchain type set proper block transactions model.
     """
     transaction_model: Type[
         Union[
@@ -291,14 +304,15 @@
             ArbitrumSepoliaTransaction,
             XaiTransaction,
             XaiSepoliaTransaction,
             AvalancheTransaction,
             AvalancheFujiTransaction,
             BlastTransaction,
             BlastSepoliaTransaction,
+            ProofOfPlayApexTransaction,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         transaction_model = EthereumTransaction
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         transaction_model = PolygonTransaction
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
@@ -327,11 +341,13 @@
         transaction_model = AvalancheTransaction
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         transaction_model = AvalancheFujiTransaction
     elif blockchain_type == AvailableBlockchainType.BLAST:
         transaction_model = BlastTransaction
     elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
         transaction_model = BlastSepoliaTransaction
+    elif blockchain_type == AvailableBlockchainType.PROOFOFPLAY_APEX:
+        transaction_model = ProofOfPlayApexTransaction
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return transaction_model
```

### Comparing `moonstreamdb-0.4.1/moonstreamdb/cli.py` & `moonstreamdb-0.4.2/moonstreamdb/cli.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.1/moonstreamdb/db.py` & `moonstreamdb-0.4.2/moonstreamdb/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.1/moonstreamdb/models.py` & `moonstreamdb-0.4.2/moonstreamdb/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1932,14 +1932,128 @@
     block_timestamp = Column(BigInteger, index=True)
     log_index = Column(Integer, nullable=True)
     created_at = Column(
         DateTime(timezone=True), server_default=utcnow(), nullable=False
     )
 
 
+class ProofOfPlayApexBlock(Base):  # type: ignore
+    __tablename__ = "proofofplay_apex_blocks"
+
+    block_number = Column(
+        BigInteger, primary_key=True, unique=True, nullable=False, index=True
+    )
+    difficulty = Column(BigInteger)
+    extra_data = Column(VARCHAR(128))
+    gas_limit = Column(BigInteger)
+    gas_used = Column(BigInteger)
+    base_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    hash = Column(VARCHAR(256), index=True)
+    logs_bloom = Column(VARCHAR(1024))
+    miner = Column(VARCHAR(256))
+    nonce = Column(VARCHAR(256))
+    parent_hash = Column(VARCHAR(256))
+    receipt_root = Column(VARCHAR(256))
+    uncles = Column(VARCHAR(256))
+    size = Column(Integer)
+    state_root = Column(VARCHAR(256))
+    timestamp = Column(BigInteger, index=True)
+    total_difficulty = Column(VARCHAR(256))
+    transactions_root = Column(VARCHAR(256))
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    sha3_uncles = Column(VARCHAR(256), nullable=True)
+    l1_block_number = Column(BigInteger, nullable=True)
+    send_count = Column(BigInteger, nullable=True)
+    send_root = Column(VARCHAR(256), nullable=True)
+    mix_hash = Column(VARCHAR(256), nullable=True)
+
+
+class ProofOfPlayApexTransaction(Base):  # type: ignore
+    __tablename__ = "proofofplay_apex_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("proofofplay_apex_blocks.block_number", ondelete="CASCADE"),
+        nullable=False,
+        index=True,
+    )
+    from_address = Column(VARCHAR(256), index=True)
+    to_address = Column(VARCHAR(256), index=True)
+    gas = Column(Numeric(precision=78, scale=0), index=True)
+    gas_price = Column(Numeric(precision=78, scale=0), index=True)
+    max_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    max_priority_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    input = Column(Text)
+    nonce = Column(VARCHAR(256))
+    transaction_index = Column(BigInteger)
+    transaction_type = Column(Integer, nullable=True)
+    value = Column(Numeric(precision=78, scale=0), index=True)
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    y_parity = Column(BigInteger, nullable=True)
+
+
+class ProofOfPlayApexLabel(Base):  # type: ignore
+    __tablename__ = "proofofplay_apex_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_proofofplay_apex_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_proofofplay_apex_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    label = Column(VARCHAR(256), nullable=False, index=True)
+    block_number = Column(
+        BigInteger,
+        nullable=True,
+        index=True,
+    )
+    address = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    transaction_hash = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    label_data = Column(JSONB, nullable=True)
+    block_timestamp = Column(BigInteger, index=True)
+    log_index = Column(Integer, nullable=True)
+    created_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
 class ESDFunctionSignature(Base):  # type: ignore
     """
     Function signature from blockchain (Ethereum/Polygon) Signature Database.
     """
 
     __tablename__ = "esd_function_signatures"
```

### Comparing `moonstreamdb-0.4.1/moonstreamdb/networks.py` & `moonstreamdb-0.4.2/moonstreamdb/networks.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     EthereumTransaction,
     MumbaiBlock,
     MumbaiLabel,
     MumbaiTransaction,
     PolygonBlock,
     PolygonLabel,
     PolygonTransaction,
+    ProofOfPlayApexBlock,
+    ProofOfPlayApexLabel,
+    ProofOfPlayApexTransaction,
     WyrmBlock,
     WyrmLabel,
     WyrmTransaction,
     XaiBlock,
     XaiLabel,
     XaiSepoliaBlock,
     XaiSepoliaLabel,
@@ -72,14 +75,15 @@
     arbitrum_sepolia = "arbitrum_sepolia"
     xai = "xai"
     xai_sepolia = "xai_sepolia"
     avalanche = "avalanche"
     avalanche_fuji = "avalanche_fuji"
     blast = "blast"
     blast_sepolia = "blast_sepolia"
+    proofofplay_apex = "proofofplay_apex"
 
 
 tx_raw_types = Union[
     EthereumTransaction,
     MumbaiTransaction,
     AmoyTransaction,
     PolygonTransaction,
@@ -92,14 +96,15 @@
     ArbitrumSepoliaTransaction,
     XaiTransaction,
     XaiSepoliaTransaction,
     AvalancheTransaction,
     AvalancheFujiTransaction,
     BlastTransaction,
     BlastSepoliaTransaction,
+    ProofOfPlayApexTransaction,
 ]
 
 MODELS: Dict[Network, Dict[str, Base]] = {
     Network.ethereum: {
         "blocks": EthereumBlock,
         "labels": EthereumLabel,
         "transactions": EthereumTransaction,
@@ -180,14 +185,19 @@
         "transactions": BlastTransaction,
     },
     Network.blast_sepolia: {
         "blocks": BlastSepoliaBlock,
         "labels": BlastSepoliaLabel,
         "transactions": BlastSepoliaTransaction,
     },
+    Network.proofofplay_apex: {
+        "blocks": ProofOfPlayApexBlock,
+        "labels": ProofOfPlayApexLabel,
+        "transactions": ProofOfPlayApexTransaction,
+    },
 }
 
 
 def blockchain_type_to_network_type(
     blockchain_type: AvailableBlockchainType,
 ) -> Network:
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
@@ -220,9 +230,11 @@
         return Network.avalanche
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         return Network.avalanche_fuji
     elif blockchain_type == AvailableBlockchainType.BLAST:
         return Network.blast
     elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
         return Network.blast_sepolia
+    elif blockchain_type == AvailableBlockchainType.PROOFOFPLAY_APEX:
+        return Network.proofofplay_apex
     else:
         raise ValueError(f"Unknown blockchain type: {blockchain_type}")
```

### Comparing `moonstreamdb-0.4.1/moonstreamdb/subscriptions.py` & `moonstreamdb-0.4.2/moonstreamdb/subscriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     ARBITRUM_SEPOLIA_BLOCKCHAIN = "arbitrum_sepolia_smartcontract"
     XAI_BLOCKCHAIN = "xai_smartcontract"
     XAI_SEPOLIA_BLOCKCHAIN = "xai_sepolia_smartcontract"
     AVALANCHE_BLOCKCHAIN = "avalanche_smartcontract"
     AVALANCHE_FUJI_BLOCKCHAIN = "avalanche_fuji_smartcontract"
     BLAST_BLOCKCHAIN = "blast_smartcontract"
     BLAST_SEPOLIA_BLOCKCHAIN = "blast_sepolia_smartcontract"
+    PROOFOFPLAY_APEX_BLOCKCHAIN = "proofofplay_apex_smartcontract"
 
 
 def blockchain_type_to_subscription_type(
     blockchain_type: AvailableBlockchainType,
 ) -> SubscriptionTypes:
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         return SubscriptionTypes.ETHEREUM_BLOCKCHAIN
@@ -56,14 +57,16 @@
         return SubscriptionTypes.AVALANCHE_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
         return SubscriptionTypes.AVALANCHE_FUJI_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.BLAST:
         return SubscriptionTypes.BLAST_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.BLAST_SEPOLIA:
         return SubscriptionTypes.BLAST_SEPOLIA_BLOCKCHAIN
+    elif blockchain_type == AvailableBlockchainType.PROOFOFPLAY_APEX:
+        return SubscriptionTypes.PROOFOFPLAY_APEX_BLOCKCHAIN
     else:
         raise ValueError(f"Unknown blockchain type: {blockchain_type}")
 
 
 subscription_id_by_blockchain = {
     "ethereum": "ethereum_smartcontract",
     "polygon": "polygon_smartcontract",
@@ -78,14 +81,15 @@
     "arbitrum_sepolia": "arbitrum_sepolia_smartcontract",
     "xai": "xai_smartcontract",
     "xai_sepolia": "xai_sepolia_smartcontract",
     "avalanche": "avalanche_smartcontract",
     "avalanche_fuji": "avalanche_fuji_smartcontract",
     "blast": "blast_smartcontract",
     "blast_sepolia": "blast_sepolia_smartcontract",
+    "proofofplay_apex": "proofofplay_apex_smartcontract",
 }
 
 blockchain_by_subscription_id = {
     "ethereum_blockchain": "ethereum",
     "polygon_blockchain": "polygon",
     "mumbai_blockchain": "mumbai",
     "amoy_blockchain": "amoy",
@@ -98,14 +102,15 @@
     "arbitrum_sepolia_blockchain": "arbitrum_sepolia",
     "xai_blockchain": "xai",
     "xai_sepolia_blockchain": "xai_sepolia",
     "avalanche_blockchain": "avalanche",
     "avalanche_fuji_blockchain": "avalanche_fuji",
     "blast_blockchain": "blast",
     "blast_sepolia_blockchain": "blast_sepolia",
+    "proofofplay_apex_blockchain": "proofofplay_apex",
     "ethereum_smartcontract": "ethereum",
     "polygon_smartcontract": "polygon",
     "mumbai_smartcontract": "mumbai",
     "amoy_smartcontract": "amoy",
     "xdai_smartcontract": "xdai",
     "wyrm_smartcontract": "wyrm",
     "zksync_era_testnet_smartcontract": "zksync_era_testnet",
@@ -115,8 +120,9 @@
     "arbitrum_sepolia_smartcontract": "arbitrum_sepolia",
     "xai_smartcontract": "xai",
     "xai_sepolia_smartcontract": "xai_sepolia",
     "avalanche_smartcontract": "avalanche",
     "avalanche_fuji_smartcontract": "avalanche_fuji",
     "blast_smartcontract": "blast",
     "blast_sepolia_smartcontract": "blast_sepolia",
+    "proofofplay_apex_smartcontract": "proofofplay_apex",
 }
```

### Comparing `moonstreamdb-0.4.1/moonstreamdb.egg-info/PKG-INFO` & `moonstreamdb-0.4.2/moonstreamdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.4.1
+Version: 0.4.2
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.4.1/setup.py` & `moonstreamdb-0.4.2/setup.py`

 * *Files identical despite different names*

