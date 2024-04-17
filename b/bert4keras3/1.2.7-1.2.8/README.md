# Comparing `tmp/bert4keras3-1.2.7-py3-none-any.whl.zip` & `tmp/bert4keras3-1.2.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59612 bytes, number of entries: 12
+Zip file size: 59678 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      150 b- defN 24-Mar-27 11:41 bert4keras3/__init__.py
 -rw-rw-rw-  2.0 fat    20229 b- defN 24-Mar-27 11:41 bert4keras3/backend.py
 -rw-rw-rw-  2.0 fat    52459 b- defN 24-Mar-27 14:03 bert4keras3/layers.py
--rw-rw-rw-  2.0 fat   123921 b- defN 24-Apr-02 12:44 bert4keras3/models.py
+-rw-rw-rw-  2.0 fat   124197 b- defN 24-Apr-17 09:13 bert4keras3/models.py
 -rw-rw-rw-  2.0 fat    30152 b- defN 24-Mar-27 11:41 bert4keras3/ops.py
 -rw-rw-rw-  2.0 fat    27955 b- defN 24-Mar-27 11:41 bert4keras3/snippets.py
 -rw-rw-rw-  2.0 fat    15509 b- defN 24-Mar-27 11:41 bert4keras3/tokenizers.py
--rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-02 13:09 bert4keras3-1.2.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      221 b- defN 24-Apr-02 13:09 bert4keras3-1.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 13:09 bert4keras3-1.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-02 13:09 bert4keras3-1.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      964 b- defN 24-Apr-02 13:09 bert4keras3-1.2.7.dist-info/RECORD
-12 files, 283022 bytes uncompressed, 58014 bytes compressed:  79.5%
+-rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-17 09:17 bert4keras3-1.2.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      221 b- defN 24-Apr-17 09:17 bert4keras3-1.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-17 09:17 bert4keras3-1.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-17 09:17 bert4keras3-1.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      965 b- defN 24-Apr-17 09:17 bert4keras3-1.2.8.dist-info/RECORD
+12 files, 283317 bytes uncompressed, 58080 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: bert4keras3/snippets.py
 Comment: 
 
 Filename: bert4keras3/tokenizers.py
 Comment: 
 
-Filename: bert4keras3-1.2.7.dist-info/LICENSE
+Filename: bert4keras3-1.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: bert4keras3-1.2.7.dist-info/METADATA
+Filename: bert4keras3-1.2.8.dist-info/METADATA
 Comment: 
 
-Filename: bert4keras3-1.2.7.dist-info/WHEEL
+Filename: bert4keras3-1.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: bert4keras3-1.2.7.dist-info/top_level.txt
+Filename: bert4keras3-1.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: bert4keras3-1.2.7.dist-info/RECORD
+Filename: bert4keras3-1.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bert4keras3/models.py

```diff
@@ -33,23 +33,23 @@
         compound_tokens=None,  # 扩展Embedding
         residual_attention_scores=False,  # Attention矩阵加残差
         ignore_invalid_weights=False,  # 允许跳过不存在的权重
         autoresize_weights=False,  # 自动变换形状不匹配的权重
         layers=None,  # 外部传入的Keras层
         prefix=None,  # 层名前缀
         name=None,  # 模型名称
-        
+        segment_attention=False,
         **kwargs
     ):
         if keep_tokens is not None:
             vocab_size = len(keep_tokens)
         if compound_tokens is not None:
             vocab_size += len(compound_tokens)
         self.vocab_size = vocab_size
-        
+        self.segment_attention = segment_attention
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
         self.num_attention_heads = num_attention_heads
         self.attention_head_size = attention_head_size or hidden_size // num_attention_heads
         self.attention_key_size = attention_key_size or self.attention_head_size
         self.intermediate_size = intermediate_size
         self.dropout_rate = dropout_rate or 0
@@ -607,19 +607,24 @@
     UniLM: https://arxiv.org/abs/1905.03197
     """
     def compute_attention_bias(self, inputs=None):
         """通过idxs序列的比较来得到对应的mask
         """
         if self.attention_bias is None:
 
-            def unilm_mask(s):
-                idxs = ops.cumsum(s, axis=1)
-                mask = idxs[:, None, :] <= idxs[:, :, None]
-                return mask
-
+            if self.segment_attention:
+                def unilm_mask(s):
+                    mask = s[:, None, :] <= s[:, :, None]
+                    return mask
+            else:
+                def unilm_mask(s):
+                    idxs = ops.cumsum(s, axis=1)
+                    mask = idxs[:, None, :] <= idxs[:, :, None]
+                    return mask
+            
             self.attention_bias = self.apply(
                 inputs=self.inputs[1],
                 layer=Lambda,
                 function=unilm_mask,
                 dtype='float32',
                 name='Attention-Mask'
             )
```

## Comparing `bert4keras3-1.2.7.dist-info/LICENSE` & `bert4keras3-1.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bert4keras3-1.2.7.dist-info/RECORD` & `bert4keras3-1.2.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 bert4keras3/__init__.py,sha256=CMb8S8X82Zw-9GhxgUom0I8qs7veKePBxPqa7nStNpk,150
 bert4keras3/backend.py,sha256=6Z7XUI2vjPtrddejf0y2rCKQftucxxCf74jjwGPs1l0,20229
 bert4keras3/layers.py,sha256=PvlMvpDjIZaIgNSJ5gfzyTgoDyK5GhhonPqJhrb16d4,52459
-bert4keras3/models.py,sha256=Rbb5tXugFCTeWc8DmYdGn3A2-dVJtpRVd5SdkCJt2pM,123921
+bert4keras3/models.py,sha256=-glWFvOSUInOZDRaeYHrA3NTM2SvSgEmmBeNyDrzN04,124197
 bert4keras3/ops.py,sha256=H1sbMv6WOJ5iGAB0rosPz9LoqdT0jS8knLRW_6XkFRU,30152
 bert4keras3/snippets.py,sha256=YwdYRvrewhM6g8ax9_Ath0HsJATzuyZksL5Dow9l65A,27955
 bert4keras3/tokenizers.py,sha256=PCxtC4L9tF2w-GUDujdPK8Z5WlnbaL8mYhRfHn1S_Qg,15509
-bert4keras3-1.2.7.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-bert4keras3-1.2.7.dist-info/METADATA,sha256=H7a0CRuXQEJWYKtjVuUXWU_nzvBRxh_d-XpjXJf_4vI,221
-bert4keras3-1.2.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-bert4keras3-1.2.7.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
-bert4keras3-1.2.7.dist-info/RECORD,,
+bert4keras3-1.2.8.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+bert4keras3-1.2.8.dist-info/METADATA,sha256=YVCq_5PRQOhq6pGuMUbnLdjojqVKiEgjMmRciC4XU2w,221
+bert4keras3-1.2.8.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+bert4keras3-1.2.8.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
+bert4keras3-1.2.8.dist-info/RECORD,,
```

