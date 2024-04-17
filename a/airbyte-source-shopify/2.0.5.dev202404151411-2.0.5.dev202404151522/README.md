# Comparing `tmp/airbyte_source_shopify-2.0.5.dev202404151411.tar.gz` & `tmp/airbyte_source_shopify-2.0.5.dev202404151522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404151411.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404151522.tar", max compression
```

## Comparing `airbyte_source_shopify-2.0.5.dev202404151411.tar` & `airbyte_source_shopify-2.0.5.dev202404151522.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4519 2024-04-15 14:08:14.682491 airbyte_source_shopify-2.0.5.dev202404151411/README.md
--rw-r--r--   0        0        0      812 2024-04-15 14:11:06.634669 airbyte_source_shopify-2.0.5.dev202404151411/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/run.py
--rw-r--r--   0        0        0    16103 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     1272 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     1009 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     1109 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0      928 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0      610 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     1170 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     1488 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     1217 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      485 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0     5313 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0      736 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0      909 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    13381 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     5226 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    14757 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     1027 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0      536 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     1329 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0      911 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    17520 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0      728 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0    80187 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     1104 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     3891 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0      907 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     2336 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0     7060 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     1675 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     4059 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0      985 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0      951 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     3750 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/scopes.py
--rw-r--r--   0        0        0     1734 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    19666 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    56188 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     3629 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-04-15 14:08:14.686491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/spec.json
--rw-r--r--   0        0        0    37308 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11968 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/transform.py
--rw-r--r--   0        0        0    13944 2024-04-15 14:08:14.694491 airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/utils.py
--rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404151411/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-15 15:19:48.877104 airbyte_source_shopify-2.0.5.dev202404151522/README.md
+-rw-r--r--   0        0        0      812 2024-04-15 15:22:43.140324 airbyte_source_shopify-2.0.5.dev202404151522/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/run.py
+-rw-r--r--   0        0        0    16103 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     1272 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     1009 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     1109 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0      928 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0      610 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     1170 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     1488 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     1217 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      485 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0     5313 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0      736 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0      909 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    13381 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     5226 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    14757 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     1027 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0      536 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     1329 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0      911 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    17520 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0      728 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0    80187 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     1104 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     3891 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0      907 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     2336 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0     7060 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     1675 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     4059 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0      985 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0      951 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     3750 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/scopes.py
+-rw-r--r--   0        0        0     1734 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    19669 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    56188 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6517 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     3629 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-04-15 15:19:48.881104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-04-15 15:19:48.889104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8540 2024-04-15 15:19:48.889104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-04-15 15:19:48.889104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/spec.json
+-rw-r--r--   0        0        0    37308 2024-04-15 15:19:48.889104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11968 2024-04-15 15:19:48.889104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-04-15 15:19:48.889104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/transform.py
+-rw-r--r--   0        0        0    13944 2024-04-15 15:19:48.889104 airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/utils.py
+-rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404151522/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/README.md` & `airbyte_source_shopify-2.0.5.dev202404151522/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/pyproject.toml` & `airbyte_source_shopify-2.0.5.dev202404151522/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.5.dev202404151411"
+version = "2.0.5.dev202404151522"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/__init__.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/auth.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/scopes.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     retrieve_chunk_size: Final[int] = 1024 * 1024 * 10
     # time between job status checks
     job_check_interval_sec: Final[int] = 2
 
     # sleep time per creation attempt
     concurrent_interval_sec: Final[int] = 30
     # max attempts for job creation
-    concurrent_max_retry: Final[int] = 30
+    concurrent_max_retry: Final[int] = 120
     # Each job ideally should be executed within the specified time (in sec),
-    # to maximize the performance for multi-connection syncs and control the bulk job size within +- 10 mins (600 sec),
+    # to maximize the performance for multi-connection syncs and control the bulk job size within +- 1 hours (3600 sec),
     # Ideally the source will balance on it's own rate, based on the time taken to return the data for the slice.
-    job_max_elapsed_time_sec: Final[float] = 600.0
+    job_max_elapsed_time_sec: Final[float] = 1800.0
     # 0.1 ~= P2H, default value, lower boundary for slice size
     job_size_min: Final[float] = 0.1
     # P365D, upper boundary for slice size
     job_size_max: Final[float] = 365.0
     # running job logger constrain
     log_job_state_msg_frequency: Final[int] = 10
     # attempt limit indicator
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/query.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/source.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/spec.json` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/streams/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/transform.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/source_shopify/utils.py` & `airbyte_source_shopify-2.0.5.dev202404151522/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404151411/PKG-INFO` & `airbyte_source_shopify-2.0.5.dev202404151522/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.0.5.dev202404151411
+Version: 2.0.5.dev202404151522
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

