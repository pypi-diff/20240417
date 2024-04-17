# Comparing `tmp/moonsdk-1.0.1.tar.gz` & `tmp/moonsdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonsdk-1.0.1.tar", max compression
+gzip compressed data, was "moonsdk-1.0.2.tar", max compression
```

## Comparing `moonsdk-1.0.1.tar` & `moonsdk-1.0.2.tar`

### file list

```diff
@@ -1,160 +1,132 @@
--rw-r--r--   0        0        0     1067 2024-04-09 02:21:20.957972 moonsdk-1.0.1/LICENSE.md
--rw-r--r--   0        0        0    21124 2024-04-17 05:18:18.685806 moonsdk-1.0.1/README.md
--rw-r--r--   0        0        0     8891 2024-04-17 03:05:52.070401 moonsdk-1.0.1/moonsdk/__init__.py
--rw-r--r--   0        0        0     1026 2024-04-17 03:05:52.077068 moonsdk-1.0.1/moonsdk/api/__init__.py
--rw-r--r--   0        0        0    45266 2024-04-17 03:05:51.710396 moonsdk-1.0.1/moonsdk/api/aave_api.py
--rw-r--r--   0        0        0   131323 2024-04-17 03:05:51.743730 moonsdk-1.0.1/moonsdk/api/accounts_api.py
--rw-r--r--   0        0        0    43718 2024-04-17 03:05:51.757063 moonsdk-1.0.1/moonsdk/api/bitcoin_api.py
--rw-r--r--   0        0        0    44213 2024-04-17 03:05:51.930399 moonsdk-1.0.1/moonsdk/api/bitcoincash_api.py
--rw-r--r--   0        0        0    12390 2024-04-17 03:05:51.767064 moonsdk-1.0.1/moonsdk/api/conveyor_finance_api.py
--rw-r--r--   0        0        0    43614 2024-04-17 03:05:51.780397 moonsdk-1.0.1/moonsdk/api/cosmos_api.py
--rw-r--r--   0        0        0    10015 2024-04-17 03:05:51.937066 moonsdk-1.0.1/moonsdk/api/default_api.py
--rw-r--r--   0        0        0    43901 2024-04-17 03:05:51.793731 moonsdk-1.0.1/moonsdk/api/doge_coin_api.py
--rw-r--r--   0        0        0    11913 2024-04-17 03:05:51.810398 moonsdk-1.0.1/moonsdk/api/ens_api.py
--rw-r--r--   0        0        0    43302 2024-04-17 03:05:51.947066 moonsdk-1.0.1/moonsdk/api/eos_api.py
--rw-r--r--   0        0        0    68599 2024-04-17 03:05:51.830398 moonsdk-1.0.1/moonsdk/api/erc1155_api.py
--rw-r--r--   0        0        0   100828 2024-04-17 03:05:51.847065 moonsdk-1.0.1/moonsdk/api/erc20_api.py
--rw-r--r--   0        0        0    23787 2024-03-18 03:51:27.816418 moonsdk-1.0.1/moonsdk/api/erc4337_api.py
--rw-r--r--   0        0        0   134851 2024-04-17 03:05:51.863732 moonsdk-1.0.1/moonsdk/api/erc721_api.py
--rw-r--r--   0        0        0    43822 2024-04-17 03:05:51.877065 moonsdk-1.0.1/moonsdk/api/litecoin_api.py
--rw-r--r--   0        0        0    61614 2024-04-17 03:05:51.960400 moonsdk-1.0.1/moonsdk/api/oneinch_api.py
--rw-r--r--   0        0        0   103849 2024-04-17 03:05:51.973733 moonsdk-1.0.1/moonsdk/api/onramper_api.py
--rw-r--r--   0        0        0   136306 2024-01-26 07:55:33.195314 moonsdk-1.0.1/moonsdk/api/payment_api.py
--rw-r--r--   0        0        0    43614 2024-04-17 03:05:51.993734 moonsdk-1.0.1/moonsdk/api/ripple_api.py
--rw-r--r--   0        0        0    43614 2024-04-17 03:05:51.890399 moonsdk-1.0.1/moonsdk/api/solana_api.py
--rw-r--r--   0        0        0    43406 2024-04-17 03:05:51.903732 moonsdk-1.0.1/moonsdk/api/tron_api.py
--rw-r--r--   0        0        0    46042 2024-04-17 03:05:51.917066 moonsdk-1.0.1/moonsdk/api/uni_swap_api.py
--rw-r--r--   0        0        0    45584 2024-04-17 03:05:52.003734 moonsdk-1.0.1/moonsdk/api/yearn_api.py
--rw-r--r--   0        0        0    25863 2024-04-17 03:05:52.083735 moonsdk-1.0.1/moonsdk/api_client.py
--rw-r--r--   0        0        0      652 2024-04-17 03:05:52.087068 moonsdk-1.0.1/moonsdk/api_response.py
--rw-r--r--   0        0        0    15639 2024-04-17 03:05:52.063735 moonsdk-1.0.1/moonsdk/configuration.py
--rw-r--r--   0        0        0     5979 2024-04-17 03:05:52.077068 moonsdk-1.0.1/moonsdk/exceptions.py
--rw-r--r--   0        0        0     7432 2024-04-17 03:05:52.073735 moonsdk-1.0.1/moonsdk/models/__init__.py
--rw-r--r--   0        0        0     4456 2024-04-17 03:05:50.720382 moonsdk-1.0.1/moonsdk/models/aave_input.py
--rw-r--r--   0        0        0     3432 2024-04-17 03:05:50.813717 moonsdk-1.0.1/moonsdk/models/aave_reserves_api_response.py
--rw-r--r--   0        0        0     3684 2024-04-17 03:05:50.820384 moonsdk-1.0.1/moonsdk/models/aave_reserves_data.py
--rw-r--r--   0        0        0     3333 2024-01-26 07:56:25.765958 moonsdk-1.0.1/moonsdk/models/abi_input.py
--rw-r--r--   0        0        0     4198 2024-01-26 07:55:32.258635 moonsdk-1.0.1/moonsdk/models/abi_item.py
--rw-r--r--   0        0        0     3233 2024-01-26 07:55:32.278636 moonsdk-1.0.1/moonsdk/models/abi_output.py
--rw-r--r--   0        0        0     3407 2024-04-17 03:05:50.833717 moonsdk-1.0.1/moonsdk/models/account_api_response.py
--rw-r--r--   0        0        0     3014 2024-01-26 07:55:32.288636 moonsdk-1.0.1/moonsdk/models/account_controller_response.py
--rw-r--r--   0        0        0    13417 2024-01-26 07:55:32.298636 moonsdk-1.0.1/moonsdk/models/account_controller_response_data.py
--rw-r--r--   0        0        0     2594 2024-04-17 03:05:50.840384 moonsdk-1.0.1/moonsdk/models/account_data.py
--rw-r--r--   0        0        0     2739 2024-04-17 03:05:50.860384 moonsdk-1.0.1/moonsdk/models/account_response.py
--rw-r--r--   0        0        0     2717 2024-04-17 03:05:50.867051 moonsdk-1.0.1/moonsdk/models/available_payment_method.py
--rw-r--r--   0        0        0     3407 2024-04-17 03:05:50.870384 moonsdk-1.0.1/moonsdk/models/balance_api_response.py
--rw-r--r--   0        0        0     2495 2024-04-17 03:05:50.877051 moonsdk-1.0.1/moonsdk/models/balance_response.py
--rw-r--r--   0        0        0     3444 2024-04-17 03:05:50.880385 moonsdk-1.0.1/moonsdk/models/bitcoin_api_response.py
--rw-r--r--   0        0        0     3477 2024-04-17 03:05:50.887051 moonsdk-1.0.1/moonsdk/models/bitcoin_cash_api_response.py
--rw-r--r--   0        0        0     2636 2024-04-17 03:05:50.890385 moonsdk-1.0.1/moonsdk/models/bitcoin_cash_input.py
--rw-r--r--   0        0        0     2892 2024-04-17 03:05:50.897051 moonsdk-1.0.1/moonsdk/models/bitcoin_cash_transaction_input.py
--rw-r--r--   0        0        0     2749 2024-04-17 03:05:50.900385 moonsdk-1.0.1/moonsdk/models/bitcoin_cash_transaction_output.py
--rw-r--r--   0        0        0     2620 2024-04-17 03:05:50.907051 moonsdk-1.0.1/moonsdk/models/bitcoin_input.py
--rw-r--r--   0        0        0     2876 2024-04-17 03:05:50.910385 moonsdk-1.0.1/moonsdk/models/bitcoin_transaction_input.py
--rw-r--r--   0        0        0     2733 2024-04-17 03:05:50.917052 moonsdk-1.0.1/moonsdk/models/bitcoin_transaction_output.py
--rw-r--r--   0        0        0     2519 2024-01-26 07:55:32.351970 moonsdk-1.0.1/moonsdk/models/block.py
--rw-r--r--   0        0        0     3538 2024-04-17 03:05:50.923718 moonsdk-1.0.1/moonsdk/models/broad_cast_raw_transaction_api_response.py
--rw-r--r--   0        0        0     2714 2024-04-17 03:05:50.927052 moonsdk-1.0.1/moonsdk/models/broad_cast_raw_transaction_response.py
--rw-r--r--   0        0        0     2662 2024-04-17 03:05:50.933719 moonsdk-1.0.1/moonsdk/models/broadcast_input.py
--rw-r--r--   0        0        0     4519 2024-04-17 03:05:50.937052 moonsdk-1.0.1/moonsdk/models/conveyor_finance_controller_response.py
--rw-r--r--   0        0        0     3436 2024-04-17 03:05:50.943719 moonsdk-1.0.1/moonsdk/models/cosmos_api_response.py
--rw-r--r--   0        0        0     2616 2024-04-17 03:05:50.963719 moonsdk-1.0.1/moonsdk/models/cosmos_input.py
--rw-r--r--   0        0        0     2872 2024-04-17 03:05:50.980386 moonsdk-1.0.1/moonsdk/models/cosmos_transaction_input.py
--rw-r--r--   0        0        0     2729 2024-04-17 03:05:50.983719 moonsdk-1.0.1/moonsdk/models/cosmos_transaction_output.py
--rw-r--r--   0        0        0     2550 2024-04-17 03:05:51.010386 moonsdk-1.0.1/moonsdk/models/create_account_input.py
--rw-r--r--   0        0        0     2880 2024-01-26 07:55:32.391970 moonsdk-1.0.1/moonsdk/models/create_payment_intent_input.py
--rw-r--r--   0        0        0     3314 2024-04-17 03:05:51.013720 moonsdk-1.0.1/moonsdk/models/crypto_currency.py
--rw-r--r--   0        0        0     2782 2024-04-17 03:05:51.020386 moonsdk-1.0.1/moonsdk/models/deploy_input.py
--rw-r--r--   0        0        0     3453 2024-04-17 03:05:51.023720 moonsdk-1.0.1/moonsdk/models/doge_coin_api_response.py
--rw-r--r--   0        0        0     2624 2024-04-17 03:05:51.027053 moonsdk-1.0.1/moonsdk/models/doge_coin_input.py
--rw-r--r--   0        0        0     2880 2024-04-17 03:05:51.030387 moonsdk-1.0.1/moonsdk/models/doge_coin_transaction_input.py
--rw-r--r--   0        0        0     2737 2024-04-17 03:05:51.037053 moonsdk-1.0.1/moonsdk/models/doge_coin_transaction_output.py
--rw-r--r--   0        0        0     3432 2024-04-17 03:05:51.040387 moonsdk-1.0.1/moonsdk/models/ens_resolve_api_response.py
--rw-r--r--   0        0        0     2572 2024-04-17 03:05:51.047053 moonsdk-1.0.1/moonsdk/models/ens_resolve_input.py
--rw-r--r--   0        0        0     2507 2024-04-17 03:05:51.053720 moonsdk-1.0.1/moonsdk/models/ens_resolve_response.py
--rw-r--r--   0        0        0     2449 2024-01-26 07:55:32.415304 moonsdk-1.0.1/moonsdk/models/ens_reverse_resolve_response.py
--rw-r--r--   0        0        0     3412 2024-04-17 03:05:51.060387 moonsdk-1.0.1/moonsdk/models/eos_api_response.py
--rw-r--r--   0        0        0     2604 2024-04-17 03:05:51.063720 moonsdk-1.0.1/moonsdk/models/eos_input.py
--rw-r--r--   0        0        0     2860 2024-04-17 03:05:51.070387 moonsdk-1.0.1/moonsdk/models/eos_transaction_input.py
--rw-r--r--   0        0        0     2717 2024-04-17 03:05:51.077054 moonsdk-1.0.1/moonsdk/models/eos_transaction_output.py
--rw-r--r--   0        0        0     3902 2024-04-17 03:05:51.090387 moonsdk-1.0.1/moonsdk/models/erc1155_request.py
--rw-r--r--   0        0        0     5611 2024-01-26 07:55:32.448638 moonsdk-1.0.1/moonsdk/models/erc1155_response.py
--rw-r--r--   0        0        0     6153 2024-01-26 07:55:32.455304 moonsdk-1.0.1/moonsdk/models/erc20_response.py
--rw-r--r--   0        0        0     3898 2024-04-17 03:05:51.093721 moonsdk-1.0.1/moonsdk/models/erc721_request.py
--rw-r--r--   0        0        0     6153 2024-01-26 07:55:32.465305 moonsdk-1.0.1/moonsdk/models/erc721_response.py
--rw-r--r--   0        0        0     2731 2024-04-17 03:05:51.100388 moonsdk-1.0.1/moonsdk/models/fiat_currency.py
--rw-r--r--   0        0        0     3098 2024-04-17 03:05:51.107054 moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response.py
--rw-r--r--   0        0        0     3245 2024-04-17 03:05:51.113721 moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response_message_inner.py
--rw-r--r--   0        0        0     3069 2024-04-17 03:05:51.117055 moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response_message_inner_icons.py
--rw-r--r--   0        0        0     2755 2024-04-17 03:05:51.120388 moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response_message_inner_icons_png.py
--rw-r--r--   0        0        0     5118 2024-04-17 03:05:51.123721 moonsdk-1.0.1/moonsdk/models/get_swap_dto.py
--rw-r--r--   0        0        0     2486 2024-01-26 07:55:32.528639 moonsdk-1.0.1/moonsdk/models/i_native_balance.py
--rw-r--r--   0        0        0     3514 2024-01-26 07:55:32.535306 moonsdk-1.0.1/moonsdk/models/i_old_nft_approval.py
--rw-r--r--   0        0        0     8889 2024-01-26 07:55:32.541972 moonsdk-1.0.1/moonsdk/models/i_webhook.py
--rw-r--r--   0        0        0     4027 2024-01-26 07:55:32.501972 moonsdk-1.0.1/moonsdk/models/ierc20_approval.py
--rw-r--r--   0        0        0     4029 2024-01-26 07:55:32.508638 moonsdk-1.0.1/moonsdk/models/ierc20_transfer.py
--rw-r--r--   0        0        0     3704 2024-01-26 07:55:32.511972 moonsdk-1.0.1/moonsdk/models/inft_approval.py
--rw-r--r--   0        0        0     3353 2024-01-26 07:55:32.518639 moonsdk-1.0.1/moonsdk/models/inft_approval_erc1155.py
--rw-r--r--   0        0        0     3350 2024-01-26 07:55:32.521972 moonsdk-1.0.1/moonsdk/models/inft_approval_erc721.py
--rw-r--r--   0        0        0     4277 2024-01-26 07:55:32.525305 moonsdk-1.0.1/moonsdk/models/inft_transfer.py
--rw-r--r--   0        0        0     3882 2024-04-17 03:05:51.130388 moonsdk-1.0.1/moonsdk/models/input_body.py
--rw-r--r--   0        0        0     3650 2024-01-26 07:55:32.551972 moonsdk-1.0.1/moonsdk/models/internal_transaction.py
--rw-r--r--   0        0        0     3452 2024-04-17 03:05:51.133721 moonsdk-1.0.1/moonsdk/models/litecoin_api_response.py
--rw-r--r--   0        0        0     2624 2024-04-17 03:05:51.137055 moonsdk-1.0.1/moonsdk/models/litecoin_input.py
--rw-r--r--   0        0        0     2880 2024-04-17 03:05:51.140388 moonsdk-1.0.1/moonsdk/models/litecoin_transaction_input.py
--rw-r--r--   0        0        0     2737 2024-04-17 03:05:51.147055 moonsdk-1.0.1/moonsdk/models/litecoin_transaction_output.py
--rw-r--r--   0        0        0     4442 2024-01-26 07:55:32.561972 moonsdk-1.0.1/moonsdk/models/log.py
--rw-r--r--   0        0        0     3407 2024-04-17 03:05:51.150388 moonsdk-1.0.1/moonsdk/models/message.py
--rw-r--r--   0        0        0     3391 2024-04-17 03:05:51.157055 moonsdk-1.0.1/moonsdk/models/nonce_api_response.py
--rw-r--r--   0        0        0     2519 2024-04-17 03:05:51.160388 moonsdk-1.0.1/moonsdk/models/nonce_response.py
--rw-r--r--   0        0        0     3442 2024-01-26 07:55:32.578639 moonsdk-1.0.1/moonsdk/models/payment_intent_response.py
--rw-r--r--   0        0        0     2673 2024-04-17 03:05:51.163722 moonsdk-1.0.1/moonsdk/models/payment_type.py
--rw-r--r--   0        0        0     2483 2024-04-17 03:05:51.170389 moonsdk-1.0.1/moonsdk/models/ping_response.py
--rw-r--r--   0        0        0     4070 2024-04-17 03:05:51.173722 moonsdk-1.0.1/moonsdk/models/quote.py
--rw-r--r--   0        0        0     3436 2024-04-17 03:05:51.180389 moonsdk-1.0.1/moonsdk/models/ripple_api_response.py
--rw-r--r--   0        0        0     2616 2024-04-17 03:05:51.183722 moonsdk-1.0.1/moonsdk/models/ripple_input.py
--rw-r--r--   0        0        0     2872 2024-04-17 03:05:51.190389 moonsdk-1.0.1/moonsdk/models/ripple_transaction_input.py
--rw-r--r--   0        0        0     2729 2024-04-17 03:05:51.197056 moonsdk-1.0.1/moonsdk/models/ripple_transaction_output.py
--rw-r--r--   0        0        0     3322 2024-04-17 03:05:51.203722 moonsdk-1.0.1/moonsdk/models/sell_quote.py
--rw-r--r--   0        0        0     2859 2024-04-17 03:05:51.207056 moonsdk-1.0.1/moonsdk/models/sign_message.py
--rw-r--r--   0        0        0     3423 2024-04-17 03:05:51.213723 moonsdk-1.0.1/moonsdk/models/sign_message_api_response.py
--rw-r--r--   0        0        0     2475 2024-04-17 03:05:51.220389 moonsdk-1.0.1/moonsdk/models/sign_typed_data.py
--rw-r--r--   0        0        0     3436 2024-04-17 03:05:51.227056 moonsdk-1.0.1/moonsdk/models/solana_api_response.py
--rw-r--r--   0        0        0     2616 2024-04-17 03:05:51.233723 moonsdk-1.0.1/moonsdk/models/solana_input.py
--rw-r--r--   0        0        0     2872 2024-04-17 03:05:51.237056 moonsdk-1.0.1/moonsdk/models/solana_transaction_input.py
--rw-r--r--   0        0        0     2729 2024-04-17 03:05:51.243723 moonsdk-1.0.1/moonsdk/models/solana_transaction_output.py
--rw-r--r--   0        0        0     3131 2024-04-17 03:05:51.250390 moonsdk-1.0.1/moonsdk/models/supported_asset_response.py
--rw-r--r--   0        0        0     2785 2024-04-17 03:05:51.257057 moonsdk-1.0.1/moonsdk/models/supported_asset_response_assets_inner.py
--rw-r--r--   0        0        0     2797 2024-04-17 03:05:51.260390 moonsdk-1.0.1/moonsdk/models/supported_currencies_response.py
--rw-r--r--   0        0        0     3387 2024-04-17 03:05:51.267057 moonsdk-1.0.1/moonsdk/models/supported_default_response.py
--rw-r--r--   0        0        0     2884 2024-04-17 03:05:51.270390 moonsdk-1.0.1/moonsdk/models/supported_default_response_defaults.py
--rw-r--r--   0        0        0     2985 2024-04-17 03:05:51.277057 moonsdk-1.0.1/moonsdk/models/supported_default_response_defaults_id.py
--rw-r--r--   0        0        0     2924 2024-04-17 03:05:51.283723 moonsdk-1.0.1/moonsdk/models/supported_payment_types_currency_response.py
--rw-r--r--   0        0        0     3486 2024-04-17 03:05:51.290390 moonsdk-1.0.1/moonsdk/models/supported_payment_types_message.py
--rw-r--r--   0        0        0     3391 2024-01-26 07:55:32.658640 moonsdk-1.0.1/moonsdk/models/tatum_transaction_event.py
--rw-r--r--   0        0        0     4836 2024-04-17 03:05:51.297057 moonsdk-1.0.1/moonsdk/models/token_swap_params.py
--rw-r--r--   0        0        0     5038 2024-04-17 03:05:51.303724 moonsdk-1.0.1/moonsdk/models/transaction.py
--rw-r--r--   0        0        0     4128 2024-04-17 03:05:51.310391 moonsdk-1.0.1/moonsdk/models/transaction_api_response.py
--rw-r--r--   0        0        0     4257 2024-04-17 03:05:51.317057 moonsdk-1.0.1/moonsdk/models/transaction_data.py
--rw-r--r--   0        0        0     4810 2024-04-17 03:05:51.323724 moonsdk-1.0.1/moonsdk/models/transaction_input.py
--rw-r--r--   0        0        0     2564 2024-04-17 03:05:51.330391 moonsdk-1.0.1/moonsdk/models/transaction_input_meta_data.py
--rw-r--r--   0        0        0     3478 2024-04-17 03:05:51.337058 moonsdk-1.0.1/moonsdk/models/transaction_input_supported_params.py
--rw-r--r--   0        0        0     3124 2024-04-17 03:05:51.343724 moonsdk-1.0.1/moonsdk/models/transaction_input_supported_params_partner_data.py
--rw-r--r--   0        0        0     2647 2024-04-17 03:05:51.350391 moonsdk-1.0.1/moonsdk/models/transaction_input_supported_params_partner_data_redirect_url.py
--rw-r--r--   0        0        0     3853 2024-04-17 03:05:51.357058 moonsdk-1.0.1/moonsdk/models/transaction_input_supported_params_theme.py
--rw-r--r--   0        0        0     2523 2024-04-17 03:05:51.360391 moonsdk-1.0.1/moonsdk/models/transaction_input_wallet.py
--rw-r--r--   0        0        0     3239 2024-04-17 03:05:51.367058 moonsdk-1.0.1/moonsdk/models/transaction_request.py
--rw-r--r--   0        0        0     3587 2024-04-17 03:05:51.373725 moonsdk-1.0.1/moonsdk/models/transaction_response.py
--rw-r--r--   0        0        0     3113 2024-04-17 03:05:51.380391 moonsdk-1.0.1/moonsdk/models/transaction_response_info.py
--rw-r--r--   0        0        0     2912 2024-04-17 03:05:51.387058 moonsdk-1.0.1/moonsdk/models/transaction_response_tx.py
--rw-r--r--   0        0        0     2679 2024-01-26 07:55:32.715308 moonsdk-1.0.1/moonsdk/models/trigger_output.py
--rw-r--r--   0        0        0     3420 2024-04-17 03:05:51.393725 moonsdk-1.0.1/moonsdk/models/tron_api_response.py
--rw-r--r--   0        0        0     2608 2024-04-17 03:05:51.400392 moonsdk-1.0.1/moonsdk/models/tron_input.py
--rw-r--r--   0        0        0     2864 2024-04-17 03:05:51.407059 moonsdk-1.0.1/moonsdk/models/tron_transaction_input.py
--rw-r--r--   0        0        0     2721 2024-04-17 03:05:51.417059 moonsdk-1.0.1/moonsdk/models/tron_transaction_output.py
--rw-r--r--   0        0        0     5385 2024-04-17 03:05:51.423725 moonsdk-1.0.1/moonsdk/models/tx.py
--rw-r--r--   0        0        0     4278 2024-04-17 03:05:51.427059 moonsdk-1.0.1/moonsdk/models/uniswap_input.py
--rw-r--r--   0        0        0        0 2024-04-17 03:05:52.060401 moonsdk-1.0.1/moonsdk/py.typed
--rw-r--r--   0        0        0     6842 2024-04-17 03:05:52.087068 moonsdk-1.0.1/moonsdk/rest.py
--rw-r--r--   0        0        0     1969 2024-04-17 05:19:05.692865 moonsdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    22134 1970-01-01 00:00:00.000000 moonsdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    21209 2024-04-17 05:20:22.160171 moonsdk-1.0.2/README.md
+-rw-r--r--   0        0        0     8891 2024-04-17 05:20:07.093378 moonsdk-1.0.2/moonsdk/__init__.py
+-rw-r--r--   0        0        0     1026 2024-04-17 05:20:07.096711 moonsdk-1.0.2/moonsdk/api/__init__.py
+-rw-r--r--   0        0        0    45266 2024-04-17 05:20:06.773376 moonsdk-1.0.2/moonsdk/api/aave_api.py
+-rw-r--r--   0        0        0   131323 2024-04-17 05:20:06.790042 moonsdk-1.0.2/moonsdk/api/accounts_api.py
+-rw-r--r--   0        0        0    43718 2024-04-17 05:20:06.803376 moonsdk-1.0.2/moonsdk/api/bitcoin_api.py
+-rw-r--r--   0        0        0    44213 2024-04-17 05:20:06.983377 moonsdk-1.0.2/moonsdk/api/bitcoincash_api.py
+-rw-r--r--   0        0        0    12390 2024-04-17 05:20:06.813376 moonsdk-1.0.2/moonsdk/api/conveyor_finance_api.py
+-rw-r--r--   0        0        0    43614 2024-04-17 05:20:06.823376 moonsdk-1.0.2/moonsdk/api/cosmos_api.py
+-rw-r--r--   0        0        0    10015 2024-04-17 05:20:06.993377 moonsdk-1.0.2/moonsdk/api/default_api.py
+-rw-r--r--   0        0        0    43901 2024-04-17 05:20:06.840043 moonsdk-1.0.2/moonsdk/api/doge_coin_api.py
+-rw-r--r--   0        0        0    11913 2024-04-17 05:20:06.853376 moonsdk-1.0.2/moonsdk/api/ens_api.py
+-rw-r--r--   0        0        0    43302 2024-04-17 05:20:07.003378 moonsdk-1.0.2/moonsdk/api/eos_api.py
+-rw-r--r--   0        0        0    68599 2024-04-17 05:20:06.870043 moonsdk-1.0.2/moonsdk/api/erc1155_api.py
+-rw-r--r--   0        0        0   100828 2024-04-17 05:20:06.893377 moonsdk-1.0.2/moonsdk/api/erc20_api.py
+-rw-r--r--   0        0        0   134851 2024-04-17 05:20:06.906710 moonsdk-1.0.2/moonsdk/api/erc721_api.py
+-rw-r--r--   0        0        0    43822 2024-04-17 05:20:06.920044 moonsdk-1.0.2/moonsdk/api/litecoin_api.py
+-rw-r--r--   0        0        0    61614 2024-04-17 05:20:07.013378 moonsdk-1.0.2/moonsdk/api/oneinch_api.py
+-rw-r--r--   0        0        0   103849 2024-04-17 05:20:07.026711 moonsdk-1.0.2/moonsdk/api/onramper_api.py
+-rw-r--r--   0        0        0    43614 2024-04-17 05:20:07.043378 moonsdk-1.0.2/moonsdk/api/ripple_api.py
+-rw-r--r--   0        0        0    43614 2024-04-17 05:20:06.933377 moonsdk-1.0.2/moonsdk/api/solana_api.py
+-rw-r--r--   0        0        0    43406 2024-04-17 05:20:06.953377 moonsdk-1.0.2/moonsdk/api/tron_api.py
+-rw-r--r--   0        0        0    46042 2024-04-17 05:20:06.970044 moonsdk-1.0.2/moonsdk/api/uni_swap_api.py
+-rw-r--r--   0        0        0    45584 2024-04-17 05:20:07.056711 moonsdk-1.0.2/moonsdk/api/yearn_api.py
+-rw-r--r--   0        0        0    25863 2024-04-17 05:20:07.103378 moonsdk-1.0.2/moonsdk/api_client.py
+-rw-r--r--   0        0        0      652 2024-04-17 05:20:07.103378 moonsdk-1.0.2/moonsdk/api_response.py
+-rw-r--r--   0        0        0    15639 2024-04-17 05:20:07.093378 moonsdk-1.0.2/moonsdk/configuration.py
+-rw-r--r--   0        0        0     5979 2024-04-17 05:20:07.100045 moonsdk-1.0.2/moonsdk/exceptions.py
+-rw-r--r--   0        0        0     7432 2024-04-17 05:20:07.096711 moonsdk-1.0.2/moonsdk/models/__init__.py
+-rw-r--r--   0        0        0     4456 2024-04-17 05:20:05.780034 moonsdk-1.0.2/moonsdk/models/aave_input.py
+-rw-r--r--   0        0        0     3432 2024-04-17 05:20:05.806701 moonsdk-1.0.2/moonsdk/models/aave_reserves_api_response.py
+-rw-r--r--   0        0        0     3684 2024-04-17 05:20:05.833368 moonsdk-1.0.2/moonsdk/models/aave_reserves_data.py
+-rw-r--r--   0        0        0     3407 2024-04-17 05:20:05.850035 moonsdk-1.0.2/moonsdk/models/account_api_response.py
+-rw-r--r--   0        0        0     2594 2024-04-17 05:20:05.873368 moonsdk-1.0.2/moonsdk/models/account_data.py
+-rw-r--r--   0        0        0     2739 2024-04-17 05:20:05.893368 moonsdk-1.0.2/moonsdk/models/account_response.py
+-rw-r--r--   0        0        0     2717 2024-04-17 05:20:05.903368 moonsdk-1.0.2/moonsdk/models/available_payment_method.py
+-rw-r--r--   0        0        0     3407 2024-04-17 05:20:05.930035 moonsdk-1.0.2/moonsdk/models/balance_api_response.py
+-rw-r--r--   0        0        0     2495 2024-04-17 05:20:05.943369 moonsdk-1.0.2/moonsdk/models/balance_response.py
+-rw-r--r--   0        0        0     3444 2024-04-17 05:20:05.953369 moonsdk-1.0.2/moonsdk/models/bitcoin_api_response.py
+-rw-r--r--   0        0        0     3477 2024-04-17 05:20:05.963369 moonsdk-1.0.2/moonsdk/models/bitcoin_cash_api_response.py
+-rw-r--r--   0        0        0     2636 2024-04-17 05:20:05.973369 moonsdk-1.0.2/moonsdk/models/bitcoin_cash_input.py
+-rw-r--r--   0        0        0     2892 2024-04-17 05:20:05.983369 moonsdk-1.0.2/moonsdk/models/bitcoin_cash_transaction_input.py
+-rw-r--r--   0        0        0     2749 2024-04-17 05:20:05.993369 moonsdk-1.0.2/moonsdk/models/bitcoin_cash_transaction_output.py
+-rw-r--r--   0        0        0     2620 2024-04-17 05:20:05.996702 moonsdk-1.0.2/moonsdk/models/bitcoin_input.py
+-rw-r--r--   0        0        0     2876 2024-04-17 05:20:06.003369 moonsdk-1.0.2/moonsdk/models/bitcoin_transaction_input.py
+-rw-r--r--   0        0        0     2733 2024-04-17 05:20:06.010036 moonsdk-1.0.2/moonsdk/models/bitcoin_transaction_output.py
+-rw-r--r--   0        0        0     3538 2024-04-17 05:20:06.016703 moonsdk-1.0.2/moonsdk/models/broad_cast_raw_transaction_api_response.py
+-rw-r--r--   0        0        0     2714 2024-04-17 05:20:06.023369 moonsdk-1.0.2/moonsdk/models/broad_cast_raw_transaction_response.py
+-rw-r--r--   0        0        0     2662 2024-04-17 05:20:06.030036 moonsdk-1.0.2/moonsdk/models/broadcast_input.py
+-rw-r--r--   0        0        0     4519 2024-04-17 05:20:06.036703 moonsdk-1.0.2/moonsdk/models/conveyor_finance_controller_response.py
+-rw-r--r--   0        0        0     3436 2024-04-17 05:20:06.046703 moonsdk-1.0.2/moonsdk/models/cosmos_api_response.py
+-rw-r--r--   0        0        0     2616 2024-04-17 05:20:06.053370 moonsdk-1.0.2/moonsdk/models/cosmos_input.py
+-rw-r--r--   0        0        0     2872 2024-04-17 05:20:06.056703 moonsdk-1.0.2/moonsdk/models/cosmos_transaction_input.py
+-rw-r--r--   0        0        0     2729 2024-04-17 05:20:06.063370 moonsdk-1.0.2/moonsdk/models/cosmos_transaction_output.py
+-rw-r--r--   0        0        0     2550 2024-04-17 05:20:06.070036 moonsdk-1.0.2/moonsdk/models/create_account_input.py
+-rw-r--r--   0        0        0     3314 2024-04-17 05:20:06.076703 moonsdk-1.0.2/moonsdk/models/crypto_currency.py
+-rw-r--r--   0        0        0     2782 2024-04-17 05:20:06.083370 moonsdk-1.0.2/moonsdk/models/deploy_input.py
+-rw-r--r--   0        0        0     3453 2024-04-17 05:20:06.090036 moonsdk-1.0.2/moonsdk/models/doge_coin_api_response.py
+-rw-r--r--   0        0        0     2624 2024-04-17 05:20:06.096703 moonsdk-1.0.2/moonsdk/models/doge_coin_input.py
+-rw-r--r--   0        0        0     2880 2024-04-17 05:20:06.106703 moonsdk-1.0.2/moonsdk/models/doge_coin_transaction_input.py
+-rw-r--r--   0        0        0     2737 2024-04-17 05:20:06.120037 moonsdk-1.0.2/moonsdk/models/doge_coin_transaction_output.py
+-rw-r--r--   0        0        0     3432 2024-04-17 05:20:06.130037 moonsdk-1.0.2/moonsdk/models/ens_resolve_api_response.py
+-rw-r--r--   0        0        0     2572 2024-04-17 05:20:06.143370 moonsdk-1.0.2/moonsdk/models/ens_resolve_input.py
+-rw-r--r--   0        0        0     2507 2024-04-17 05:20:06.150037 moonsdk-1.0.2/moonsdk/models/ens_resolve_response.py
+-rw-r--r--   0        0        0     3412 2024-04-17 05:20:06.166704 moonsdk-1.0.2/moonsdk/models/eos_api_response.py
+-rw-r--r--   0        0        0     2604 2024-04-17 05:20:06.176704 moonsdk-1.0.2/moonsdk/models/eos_input.py
+-rw-r--r--   0        0        0     2860 2024-04-17 05:20:06.183371 moonsdk-1.0.2/moonsdk/models/eos_transaction_input.py
+-rw-r--r--   0        0        0     2717 2024-04-17 05:20:06.193371 moonsdk-1.0.2/moonsdk/models/eos_transaction_output.py
+-rw-r--r--   0        0        0     3902 2024-04-17 05:20:06.200037 moonsdk-1.0.2/moonsdk/models/erc1155_request.py
+-rw-r--r--   0        0        0     3898 2024-04-17 05:20:06.210038 moonsdk-1.0.2/moonsdk/models/erc721_request.py
+-rw-r--r--   0        0        0     2731 2024-04-17 05:20:06.216704 moonsdk-1.0.2/moonsdk/models/fiat_currency.py
+-rw-r--r--   0        0        0     3098 2024-04-17 05:20:06.226704 moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response.py
+-rw-r--r--   0        0        0     3245 2024-04-17 05:20:06.230038 moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response_message_inner.py
+-rw-r--r--   0        0        0     3069 2024-04-17 05:20:06.236704 moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response_message_inner_icons.py
+-rw-r--r--   0        0        0     2755 2024-04-17 05:20:06.240038 moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response_message_inner_icons_png.py
+-rw-r--r--   0        0        0     5118 2024-04-17 05:20:06.243371 moonsdk-1.0.2/moonsdk/models/get_swap_dto.py
+-rw-r--r--   0        0        0     3882 2024-04-17 05:20:06.250038 moonsdk-1.0.2/moonsdk/models/input_body.py
+-rw-r--r--   0        0        0     3452 2024-04-17 05:20:06.253371 moonsdk-1.0.2/moonsdk/models/litecoin_api_response.py
+-rw-r--r--   0        0        0     2624 2024-04-17 05:20:06.256705 moonsdk-1.0.2/moonsdk/models/litecoin_input.py
+-rw-r--r--   0        0        0     2880 2024-04-17 05:20:06.263371 moonsdk-1.0.2/moonsdk/models/litecoin_transaction_input.py
+-rw-r--r--   0        0        0     2737 2024-04-17 05:20:06.266705 moonsdk-1.0.2/moonsdk/models/litecoin_transaction_output.py
+-rw-r--r--   0        0        0     3407 2024-04-17 05:20:06.270038 moonsdk-1.0.2/moonsdk/models/message.py
+-rw-r--r--   0        0        0     3391 2024-04-17 05:20:06.276705 moonsdk-1.0.2/moonsdk/models/nonce_api_response.py
+-rw-r--r--   0        0        0     2519 2024-04-17 05:20:06.280038 moonsdk-1.0.2/moonsdk/models/nonce_response.py
+-rw-r--r--   0        0        0     2673 2024-04-17 05:20:06.286705 moonsdk-1.0.2/moonsdk/models/payment_type.py
+-rw-r--r--   0        0        0     2483 2024-04-17 05:20:06.290038 moonsdk-1.0.2/moonsdk/models/ping_response.py
+-rw-r--r--   0        0        0     4070 2024-04-17 05:20:06.296705 moonsdk-1.0.2/moonsdk/models/quote.py
+-rw-r--r--   0        0        0     3436 2024-04-17 05:20:06.300038 moonsdk-1.0.2/moonsdk/models/ripple_api_response.py
+-rw-r--r--   0        0        0     2616 2024-04-17 05:20:06.303372 moonsdk-1.0.2/moonsdk/models/ripple_input.py
+-rw-r--r--   0        0        0     2872 2024-04-17 05:20:06.306705 moonsdk-1.0.2/moonsdk/models/ripple_transaction_input.py
+-rw-r--r--   0        0        0     2729 2024-04-17 05:20:06.313372 moonsdk-1.0.2/moonsdk/models/ripple_transaction_output.py
+-rw-r--r--   0        0        0     3322 2024-04-17 05:20:06.316705 moonsdk-1.0.2/moonsdk/models/sell_quote.py
+-rw-r--r--   0        0        0     2859 2024-04-17 05:20:06.320038 moonsdk-1.0.2/moonsdk/models/sign_message.py
+-rw-r--r--   0        0        0     3423 2024-04-17 05:20:06.330038 moonsdk-1.0.2/moonsdk/models/sign_message_api_response.py
+-rw-r--r--   0        0        0     2475 2024-04-17 05:20:06.333372 moonsdk-1.0.2/moonsdk/models/sign_typed_data.py
+-rw-r--r--   0        0        0     3436 2024-04-17 05:20:06.336705 moonsdk-1.0.2/moonsdk/models/solana_api_response.py
+-rw-r--r--   0        0        0     2616 2024-04-17 05:20:06.343372 moonsdk-1.0.2/moonsdk/models/solana_input.py
+-rw-r--r--   0        0        0     2872 2024-04-17 05:20:06.346705 moonsdk-1.0.2/moonsdk/models/solana_transaction_input.py
+-rw-r--r--   0        0        0     2729 2024-04-17 05:20:06.350039 moonsdk-1.0.2/moonsdk/models/solana_transaction_output.py
+-rw-r--r--   0        0        0     3131 2024-04-17 05:20:06.356706 moonsdk-1.0.2/moonsdk/models/supported_asset_response.py
+-rw-r--r--   0        0        0     2785 2024-04-17 05:20:06.360039 moonsdk-1.0.2/moonsdk/models/supported_asset_response_assets_inner.py
+-rw-r--r--   0        0        0     2797 2024-04-17 05:20:06.366706 moonsdk-1.0.2/moonsdk/models/supported_currencies_response.py
+-rw-r--r--   0        0        0     3387 2024-04-17 05:20:06.373372 moonsdk-1.0.2/moonsdk/models/supported_default_response.py
+-rw-r--r--   0        0        0     2884 2024-04-17 05:20:06.380039 moonsdk-1.0.2/moonsdk/models/supported_default_response_defaults.py
+-rw-r--r--   0        0        0     2985 2024-04-17 05:20:06.386706 moonsdk-1.0.2/moonsdk/models/supported_default_response_defaults_id.py
+-rw-r--r--   0        0        0     2924 2024-04-17 05:20:06.393372 moonsdk-1.0.2/moonsdk/models/supported_payment_types_currency_response.py
+-rw-r--r--   0        0        0     3486 2024-04-17 05:20:06.403372 moonsdk-1.0.2/moonsdk/models/supported_payment_types_message.py
+-rw-r--r--   0        0        0     4836 2024-04-17 05:20:06.410039 moonsdk-1.0.2/moonsdk/models/token_swap_params.py
+-rw-r--r--   0        0        0     5038 2024-04-17 05:20:06.416706 moonsdk-1.0.2/moonsdk/models/transaction.py
+-rw-r--r--   0        0        0     4128 2024-04-17 05:20:06.420039 moonsdk-1.0.2/moonsdk/models/transaction_api_response.py
+-rw-r--r--   0        0        0     4257 2024-04-17 05:20:06.430039 moonsdk-1.0.2/moonsdk/models/transaction_data.py
+-rw-r--r--   0        0        0     4810 2024-04-17 05:20:06.433373 moonsdk-1.0.2/moonsdk/models/transaction_input.py
+-rw-r--r--   0        0        0     2564 2024-04-17 05:20:06.440039 moonsdk-1.0.2/moonsdk/models/transaction_input_meta_data.py
+-rw-r--r--   0        0        0     3478 2024-04-17 05:20:06.446706 moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params.py
+-rw-r--r--   0        0        0     3124 2024-04-17 05:20:06.453373 moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params_partner_data.py
+-rw-r--r--   0        0        0     2647 2024-04-17 05:20:06.460040 moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params_partner_data_redirect_url.py
+-rw-r--r--   0        0        0     3853 2024-04-17 05:20:06.463373 moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params_theme.py
+-rw-r--r--   0        0        0     2523 2024-04-17 05:20:06.466706 moonsdk-1.0.2/moonsdk/models/transaction_input_wallet.py
+-rw-r--r--   0        0        0     3239 2024-04-17 05:20:06.473373 moonsdk-1.0.2/moonsdk/models/transaction_request.py
+-rw-r--r--   0        0        0     3587 2024-04-17 05:20:06.473373 moonsdk-1.0.2/moonsdk/models/transaction_response.py
+-rw-r--r--   0        0        0     3113 2024-04-17 05:20:06.476706 moonsdk-1.0.2/moonsdk/models/transaction_response_info.py
+-rw-r--r--   0        0        0     2912 2024-04-17 05:20:06.480040 moonsdk-1.0.2/moonsdk/models/transaction_response_tx.py
+-rw-r--r--   0        0        0     3420 2024-04-17 05:20:06.483373 moonsdk-1.0.2/moonsdk/models/tron_api_response.py
+-rw-r--r--   0        0        0     2608 2024-04-17 05:20:06.486707 moonsdk-1.0.2/moonsdk/models/tron_input.py
+-rw-r--r--   0        0        0     2864 2024-04-17 05:20:06.490040 moonsdk-1.0.2/moonsdk/models/tron_transaction_input.py
+-rw-r--r--   0        0        0     2721 2024-04-17 05:20:06.493373 moonsdk-1.0.2/moonsdk/models/tron_transaction_output.py
+-rw-r--r--   0        0        0     5385 2024-04-17 05:20:06.496707 moonsdk-1.0.2/moonsdk/models/tx.py
+-rw-r--r--   0        0        0     4278 2024-04-17 05:20:06.500040 moonsdk-1.0.2/moonsdk/models/uniswap_input.py
+-rw-r--r--   0        0        0        0 2024-04-17 05:20:07.090045 moonsdk-1.0.2/moonsdk/py.typed
+-rw-r--r--   0        0        0     6842 2024-04-17 05:20:07.106712 moonsdk-1.0.2/moonsdk/rest.py
+-rw-r--r--   0        0        0     1969 2024-04-17 05:20:22.160171 moonsdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    22219 1970-01-01 00:00:00.000000 moonsdk-1.0.2/PKG-INFO
```

### Comparing `moonsdk-1.0.1/README.md` & `moonsdk-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install moonsdk 
+pip install git+https://github.com/moon-up/moon-sdk-python.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install moonsdk`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/moon-up/moon-sdk-python.git`)
 
 Then import the package:
 ```python
 import moonsdk
 ```
 
 ### Setuptools
```

### Comparing `moonsdk-1.0.1/moonsdk/__init__.py` & `moonsdk-1.0.2/moonsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/__init__.py` & `moonsdk-1.0.2/moonsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/aave_api.py` & `moonsdk-1.0.2/moonsdk/api/aave_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/accounts_api.py` & `moonsdk-1.0.2/moonsdk/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/bitcoin_api.py` & `moonsdk-1.0.2/moonsdk/api/bitcoin_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/bitcoincash_api.py` & `moonsdk-1.0.2/moonsdk/api/bitcoincash_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/conveyor_finance_api.py` & `moonsdk-1.0.2/moonsdk/api/conveyor_finance_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/cosmos_api.py` & `moonsdk-1.0.2/moonsdk/api/cosmos_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/default_api.py` & `moonsdk-1.0.2/moonsdk/api/default_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/doge_coin_api.py` & `moonsdk-1.0.2/moonsdk/api/doge_coin_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/ens_api.py` & `moonsdk-1.0.2/moonsdk/api/ens_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/eos_api.py` & `moonsdk-1.0.2/moonsdk/api/eos_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/erc1155_api.py` & `moonsdk-1.0.2/moonsdk/api/erc1155_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/erc20_api.py` & `moonsdk-1.0.2/moonsdk/api/erc20_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/erc4337_api.py` & `moonsdk-1.0.2/moonsdk/api/yearn_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,76 +7,67 @@
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
-
-import io
 import warnings
-
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
-from typing import Dict, List, Optional, Tuple, Union, Any
-
-try:
-    from typing import Annotated
-except ImportError:
-    from typing_extensions import Annotated
+from typing import Any, Dict, List, Optional, Tuple, Union
+from typing_extensions import Annotated
 
 from pydantic import StrictStr
-
-from moonsdk.models.account_api_response import AccountAPIResponse
 from moonsdk.models.input_body import InputBody
 from moonsdk.models.transaction_api_response import TransactionAPIResponse
 
-from moonsdk.api_client import ApiClient
+from moonsdk.api_client import ApiClient, RequestSerialized
 from moonsdk.api_response import ApiResponse
 from moonsdk.rest import RESTResponseType
 
 
-class Erc4337Api:
+class YearnApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    async def get_address(
+    async def add_liquidity(
         self,
         authorization: StrictStr,
-        account_name: StrictStr,
+        name: StrictStr,
         input_body: InputBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> AccountAPIResponse:
-        """get_address
+    ) -> TransactionAPIResponse:
+        """add_liquidity
 
 
         :param authorization: (required)
         :type authorization: str
-        :param account_name: (required)
-        :type account_name: str
+        :param name: (required)
+        :type name: str
         :param input_body: (required)
         :type input_body: InputBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -93,64 +84,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_address_serialize(
+        _param = self._add_liquidity_serialize(
             authorization=authorization,
-            account_name=account_name,
+            name=name,
             input_body=input_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AccountAPIResponse",
+            '200': "TransactionAPIResponse",
         }
         response_data = await self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         await response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    async def get_address_with_http_info(
+    async def add_liquidity_with_http_info(
         self,
         authorization: StrictStr,
-        account_name: StrictStr,
+        name: StrictStr,
         input_body: InputBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[AccountAPIResponse]:
-        """get_address
+    ) -> ApiResponse[TransactionAPIResponse]:
+        """add_liquidity
 
 
         :param authorization: (required)
         :type authorization: str
-        :param account_name: (required)
-        :type account_name: str
+        :param name: (required)
+        :type name: str
         :param input_body: (required)
         :type input_body: InputBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -167,64 +158,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_address_serialize(
+        _param = self._add_liquidity_serialize(
             authorization=authorization,
-            account_name=account_name,
+            name=name,
             input_body=input_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AccountAPIResponse",
+            '200': "TransactionAPIResponse",
         }
         response_data = await self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         await response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    async def get_address_without_preload_content(
+    async def add_liquidity_without_preload_content(
         self,
         authorization: StrictStr,
-        account_name: StrictStr,
+        name: StrictStr,
         input_body: InputBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """get_address
+        """add_liquidity
 
 
         :param authorization: (required)
         :type authorization: str
-        :param account_name: (required)
-        :type account_name: str
+        :param name: (required)
+        :type name: str
         :param input_body: (required)
         :type input_body: InputBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -241,60 +232,658 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_address_serialize(
+        _param = self._add_liquidity_serialize(
             authorization=authorization,
-            account_name=account_name,
+            name=name,
             input_body=input_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "AccountAPIResponse",
+            '200': "TransactionAPIResponse",
+        }
+        response_data = await self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _add_liquidity_serialize(
+        self,
+        authorization,
+        name,
+        input_body,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if name is not None:
+            _path_params['name'] = name
+        # process the query parameters
+        # process the header parameters
+        if authorization is not None:
+            _header_params['Authorization'] = authorization
+        # process the form parameters
+        # process the body parameter
+        if input_body is not None:
+            _body_params = input_body
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth', 
+            'BearerAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/yearn/{name}/add-liquidity',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    async def add_liquidity_weth(
+        self,
+        authorization: StrictStr,
+        name: StrictStr,
+        input_body: InputBody,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> TransactionAPIResponse:
+        """add_liquidity_weth
+
+
+        :param authorization: (required)
+        :type authorization: str
+        :param name: (required)
+        :type name: str
+        :param input_body: (required)
+        :type input_body: InputBody
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._add_liquidity_weth_serialize(
+            authorization=authorization,
+            name=name,
+            input_body=input_body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TransactionAPIResponse",
+        }
+        response_data = await self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        await response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    async def add_liquidity_weth_with_http_info(
+        self,
+        authorization: StrictStr,
+        name: StrictStr,
+        input_body: InputBody,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[TransactionAPIResponse]:
+        """add_liquidity_weth
+
+
+        :param authorization: (required)
+        :type authorization: str
+        :param name: (required)
+        :type name: str
+        :param input_body: (required)
+        :type input_body: InputBody
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._add_liquidity_weth_serialize(
+            authorization=authorization,
+            name=name,
+            input_body=input_body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TransactionAPIResponse",
+        }
+        response_data = await self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        await response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    async def add_liquidity_weth_without_preload_content(
+        self,
+        authorization: StrictStr,
+        name: StrictStr,
+        input_body: InputBody,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """add_liquidity_weth
+
+
+        :param authorization: (required)
+        :type authorization: str
+        :param name: (required)
+        :type name: str
+        :param input_body: (required)
+        :type input_body: InputBody
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._add_liquidity_weth_serialize(
+            authorization=authorization,
+            name=name,
+            input_body=input_body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TransactionAPIResponse",
+        }
+        response_data = await self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _add_liquidity_weth_serialize(
+        self,
+        authorization,
+        name,
+        input_body,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if name is not None:
+            _path_params['name'] = name
+        # process the query parameters
+        # process the header parameters
+        if authorization is not None:
+            _header_params['Authorization'] = authorization
+        # process the form parameters
+        # process the body parameter
+        if input_body is not None:
+            _body_params = input_body
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'ApiKeyAuth', 
+            'BearerAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/yearn/{name}/add-liquidity-weth',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    async def remove_liquidity(
+        self,
+        authorization: StrictStr,
+        name: StrictStr,
+        input_body: InputBody,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> TransactionAPIResponse:
+        """remove_liquidity
+
+
+        :param authorization: (required)
+        :type authorization: str
+        :param name: (required)
+        :type name: str
+        :param input_body: (required)
+        :type input_body: InputBody
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._remove_liquidity_serialize(
+            authorization=authorization,
+            name=name,
+            input_body=input_body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TransactionAPIResponse",
+        }
+        response_data = await self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        await response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    async def remove_liquidity_with_http_info(
+        self,
+        authorization: StrictStr,
+        name: StrictStr,
+        input_body: InputBody,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[TransactionAPIResponse]:
+        """remove_liquidity
+
+
+        :param authorization: (required)
+        :type authorization: str
+        :param name: (required)
+        :type name: str
+        :param input_body: (required)
+        :type input_body: InputBody
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._remove_liquidity_serialize(
+            authorization=authorization,
+            name=name,
+            input_body=input_body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TransactionAPIResponse",
+        }
+        response_data = await self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        await response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    async def remove_liquidity_without_preload_content(
+        self,
+        authorization: StrictStr,
+        name: StrictStr,
+        input_body: InputBody,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """remove_liquidity
+
+
+        :param authorization: (required)
+        :type authorization: str
+        :param name: (required)
+        :type name: str
+        :param input_body: (required)
+        :type input_body: InputBody
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._remove_liquidity_serialize(
+            authorization=authorization,
+            name=name,
+            input_body=input_body,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "TransactionAPIResponse",
         }
         response_data = await self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_address_serialize(
+    def _remove_liquidity_serialize(
         self,
         authorization,
-        account_name,
+        name,
         input_body,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
-    ) -> Tuple:
+    ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if account_name is not None:
-            _path_params['accountName'] = account_name
+        if name is not None:
+            _path_params['name'] = name
         # process the query parameters
         # process the header parameters
         if authorization is not None:
             _header_params['Authorization'] = authorization
         # process the form parameters
         # process the body parameter
         if input_body is not None:
@@ -326,15 +915,15 @@
         _auth_settings: List[str] = [
             'ApiKeyAuth', 
             'BearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/erc4337/{accountName}/address',
+            resource_path='/yearn/{name}/remove-liquidity',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -343,39 +932,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    async def sign_broadcast_user_op_tx(
+    async def remove_liquidity_weth(
         self,
         authorization: StrictStr,
-        account_name: StrictStr,
+        name: StrictStr,
         input_body: InputBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> TransactionAPIResponse:
-        """sign_broadcast_user_op_tx
+        """remove_liquidity_weth
 
 
         :param authorization: (required)
         :type authorization: str
-        :param account_name: (required)
-        :type account_name: str
+        :param name: (required)
+        :type name: str
         :param input_body: (required)
         :type input_body: InputBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -392,17 +981,17 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._sign_broadcast_user_op_tx_serialize(
+        _param = self._remove_liquidity_weth_serialize(
             authorization=authorization,
-            account_name=account_name,
+            name=name,
             input_body=input_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -417,39 +1006,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    async def sign_broadcast_user_op_tx_with_http_info(
+    async def remove_liquidity_weth_with_http_info(
         self,
         authorization: StrictStr,
-        account_name: StrictStr,
+        name: StrictStr,
         input_body: InputBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[TransactionAPIResponse]:
-        """sign_broadcast_user_op_tx
+        """remove_liquidity_weth
 
 
         :param authorization: (required)
         :type authorization: str
-        :param account_name: (required)
-        :type account_name: str
+        :param name: (required)
+        :type name: str
         :param input_body: (required)
         :type input_body: InputBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -466,17 +1055,17 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._sign_broadcast_user_op_tx_serialize(
+        _param = self._remove_liquidity_weth_serialize(
             authorization=authorization,
-            account_name=account_name,
+            name=name,
             input_body=input_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -491,39 +1080,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    async def sign_broadcast_user_op_tx_without_preload_content(
+    async def remove_liquidity_weth_without_preload_content(
         self,
         authorization: StrictStr,
-        account_name: StrictStr,
+        name: StrictStr,
         input_body: InputBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """sign_broadcast_user_op_tx
+        """remove_liquidity_weth
 
 
         :param authorization: (required)
         :type authorization: str
-        :param account_name: (required)
-        :type account_name: str
+        :param name: (required)
+        :type name: str
         :param input_body: (required)
         :type input_body: InputBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -540,17 +1129,17 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._sign_broadcast_user_op_tx_serialize(
+        _param = self._remove_liquidity_weth_serialize(
             authorization=authorization,
-            account_name=account_name,
+            name=name,
             input_body=input_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -560,40 +1149,40 @@
         response_data = await self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _sign_broadcast_user_op_tx_serialize(
+    def _remove_liquidity_weth_serialize(
         self,
         authorization,
-        account_name,
+        name,
         input_body,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
-    ) -> Tuple:
+    ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if account_name is not None:
-            _path_params['accountName'] = account_name
+        if name is not None:
+            _path_params['name'] = name
         # process the query parameters
         # process the header parameters
         if authorization is not None:
             _header_params['Authorization'] = authorization
         # process the form parameters
         # process the body parameter
         if input_body is not None:
@@ -625,15 +1214,15 @@
         _auth_settings: List[str] = [
             'ApiKeyAuth', 
             'BearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/erc4337/{accountName}/sign-broadcast-userop-tx',
+            resource_path='/yearn/{name}/remove-liquidity-weth',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `moonsdk-1.0.1/moonsdk/api/erc721_api.py` & `moonsdk-1.0.2/moonsdk/api/erc721_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/litecoin_api.py` & `moonsdk-1.0.2/moonsdk/api/litecoin_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/oneinch_api.py` & `moonsdk-1.0.2/moonsdk/api/oneinch_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/onramper_api.py` & `moonsdk-1.0.2/moonsdk/api/onramper_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/ripple_api.py` & `moonsdk-1.0.2/moonsdk/api/ripple_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/solana_api.py` & `moonsdk-1.0.2/moonsdk/api/solana_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/tron_api.py` & `moonsdk-1.0.2/moonsdk/api/tron_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api/uni_swap_api.py` & `moonsdk-1.0.2/moonsdk/api/uni_swap_api.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api_client.py` & `moonsdk-1.0.2/moonsdk/api_client.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/api_response.py` & `moonsdk-1.0.2/moonsdk/api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/configuration.py` & `moonsdk-1.0.2/moonsdk/configuration.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/exceptions.py` & `moonsdk-1.0.2/moonsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/__init__.py` & `moonsdk-1.0.2/moonsdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/aave_input.py` & `moonsdk-1.0.2/moonsdk/models/aave_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/aave_reserves_api_response.py` & `moonsdk-1.0.2/moonsdk/models/aave_reserves_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/aave_reserves_data.py` & `moonsdk-1.0.2/moonsdk/models/aave_reserves_data.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/abi_input.py` & `moonsdk-1.0.2/moonsdk/models/ens_resolve_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,94 +13,75 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictBool, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class AbiInput(BaseModel):
+class EnsResolveResponse(BaseModel):
     """
-    AbiInput
+    EnsResolveResponse
     """ # noqa: E501
-    name: StrictStr
-    type: StrictStr
-    indexed: Optional[StrictBool] = None
-    components: Optional[List[AbiInput]] = None
-    internal_type: Optional[StrictStr] = Field(default=None, alias="internalType")
-    __properties: ClassVar[List[str]] = ["name", "type", "indexed", "components", "internalType"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    address: StrictStr
+    __properties: ClassVar[List[str]] = ["address"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AbiInput from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of EnsResolveResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in components (list)
-        _items = []
-        if self.components:
-            for _item in self.components:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['components'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of AbiInput from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of EnsResolveResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "type": obj.get("type"),
-            "indexed": obj.get("indexed"),
-            "components": [AbiInput.from_dict(_item) for _item in obj.get("components")] if obj.get("components") is not None else None,
-            "internalType": obj.get("internalType")
+            "address": obj.get("address")
         })
         return _obj
 
-# TODO: Rewrite to not use raise_errors
-AbiInput.model_rebuild(raise_errors=False)
```

### Comparing `moonsdk-1.0.1/moonsdk/models/abi_item.py` & `moonsdk-1.0.2/moonsdk/models/broad_cast_raw_transaction_api_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,109 +13,91 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from moonsdk.models.broad_cast_raw_transaction_response import BroadCastRawTransactionResponse
+from moonsdk.models.input_body import InputBody
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from pydantic import BaseModel, StrictBool, StrictFloat, StrictInt, StrictStr
-from pydantic import Field
-from moonsdk.models.abi_input import AbiInput
-from moonsdk.models.abi_output import AbiOutput
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class AbiItem(BaseModel):
+class BroadCastRawTransactionAPIResponse(BaseModel):
     """
-    The abi to parse the log object of the contract
+    BroadCastRawTransactionAPIResponse
     """ # noqa: E501
-    anonymous: Optional[StrictBool] = None
-    constant: Optional[StrictBool] = None
-    inputs: Optional[List[AbiInput]] = None
-    name: Optional[StrictStr] = None
-    outputs: Optional[List[AbiOutput]] = None
-    payable: Optional[StrictBool] = None
-    state_mutability: Optional[StrictStr] = Field(default=None, alias="stateMutability")
-    type: StrictStr
-    gas: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties: ClassVar[List[str]] = ["anonymous", "constant", "inputs", "name", "outputs", "payable", "stateMutability", "type", "gas"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    success: StrictBool
+    message: StrictStr
+    body: Optional[InputBody] = None
+    address: Optional[StrictStr] = None
+    data: Optional[BroadCastRawTransactionResponse] = None
+    __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AbiItem from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of BroadCastRawTransactionAPIResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in inputs (list)
-        _items = []
-        if self.inputs:
-            for _item in self.inputs:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['inputs'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in outputs (list)
-        _items = []
-        if self.outputs:
-            for _item in self.outputs:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['outputs'] = _items
+        # override the default output from pydantic by calling `to_dict()` of body
+        if self.body:
+            _dict['body'] = self.body.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of AbiItem from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of BroadCastRawTransactionAPIResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "anonymous": obj.get("anonymous"),
-            "constant": obj.get("constant"),
-            "inputs": [AbiInput.from_dict(_item) for _item in obj.get("inputs")] if obj.get("inputs") is not None else None,
-            "name": obj.get("name"),
-            "outputs": [AbiOutput.from_dict(_item) for _item in obj.get("outputs")] if obj.get("outputs") is not None else None,
-            "payable": obj.get("payable"),
-            "stateMutability": obj.get("stateMutability"),
-            "type": obj.get("type"),
-            "gas": obj.get("gas")
+            "success": obj.get("success"),
+            "message": obj.get("message"),
+            "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
+            "address": obj.get("address"),
+            "data": BroadCastRawTransactionResponse.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/abi_output.py` & `moonsdk-1.0.2/moonsdk/models/message.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,92 +13,93 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List
+from moonsdk.models.crypto_currency import CryptoCurrency
+from moonsdk.models.fiat_currency import FiatCurrency
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class AbiOutput(BaseModel):
+class Message(BaseModel):
     """
-    AbiOutput
+    Message
     """ # noqa: E501
-    name: StrictStr
-    type: StrictStr
-    components: Optional[List[AbiOutput]] = None
-    internal_type: Optional[StrictStr] = Field(default=None, alias="internalType")
-    __properties: ClassVar[List[str]] = ["name", "type", "components", "internalType"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    fiat: List[FiatCurrency]
+    crypto: List[CryptoCurrency]
+    __properties: ClassVar[List[str]] = ["fiat", "crypto"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AbiOutput from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in components (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in fiat (list)
+        _items = []
+        if self.fiat:
+            for _item in self.fiat:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['fiat'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in crypto (list)
         _items = []
-        if self.components:
-            for _item in self.components:
+        if self.crypto:
+            for _item in self.crypto:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['components'] = _items
+            _dict['crypto'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of AbiOutput from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of Message from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "type": obj.get("type"),
-            "components": [AbiOutput.from_dict(_item) for _item in obj.get("components")] if obj.get("components") is not None else None,
-            "internalType": obj.get("internalType")
+            "fiat": [FiatCurrency.from_dict(_item) for _item in obj["fiat"]] if obj.get("fiat") is not None else None,
+            "crypto": [CryptoCurrency.from_dict(_item) for _item in obj["crypto"]] if obj.get("crypto") is not None else None
         })
         return _obj
 
-# TODO: Rewrite to not use raise_errors
-AbiOutput.model_rebuild(raise_errors=False)
```

### Comparing `moonsdk-1.0.1/moonsdk/models/account_api_response.py` & `moonsdk-1.0.2/moonsdk/models/account_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/account_controller_response.py` & `moonsdk-1.0.2/moonsdk/models/account_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,84 +13,79 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List
+from moonsdk.models.account_data import AccountData
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictBool, StrictStr
-from moonsdk.models.account_controller_response_data import AccountControllerResponseData
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class AccountControllerResponse(BaseModel):
+class AccountResponse(BaseModel):
     """
-    AccountControllerResponse
+    AccountResponse
     """ # noqa: E501
-    data: Optional[AccountControllerResponseData] = None
-    success: Optional[StrictBool] = None
-    message: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["data", "success", "message"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    data: AccountData
+    __properties: ClassVar[List[str]] = ["data"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AccountControllerResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of AccountResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of AccountControllerResponse from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of AccountResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "data": AccountControllerResponseData.from_dict(obj.get("data")) if obj.get("data") is not None else None,
-            "success": obj.get("success"),
-            "message": obj.get("message")
+            "data": AccountData.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/account_data.py` & `moonsdk-1.0.2/moonsdk/models/account_data.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/account_response.py` & `moonsdk-1.0.2/moonsdk/models/sign_typed_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,24 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from moonsdk.models.account_data import AccountData
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AccountResponse(BaseModel):
+class SignTypedData(BaseModel):
     """
-    AccountResponse
+    SignTypedData
     """ # noqa: E501
-    data: AccountData
+    data: StrictStr
     __properties: ClassVar[List[str]] = ["data"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -44,15 +43,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AccountResponse from a JSON string"""
+        """Create an instance of SignTypedData from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,27 +64,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of data
-        if self.data:
-            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AccountResponse from a dict"""
+        """Create an instance of SignTypedData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "data": AccountData.from_dict(obj["data"]) if obj.get("data") is not None else None
+            "data": obj.get("data")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/available_payment_method.py` & `moonsdk-1.0.2/moonsdk/models/available_payment_method.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/balance_api_response.py` & `moonsdk-1.0.2/moonsdk/models/balance_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/balance_response.py` & `moonsdk-1.0.2/moonsdk/models/balance_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_api_response.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_cash_api_response.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_cash_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_cash_input.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_cash_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_cash_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_cash_transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_cash_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_cash_transaction_output.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_input.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/bitcoin_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/bitcoin_transaction_output.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/block.py` & `moonsdk-1.0.2/moonsdk/models/doge_coin_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,80 +13,77 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class Block(BaseModel):
+class DogeCoinInput(BaseModel):
     """
-    Block
+    DogeCoinInput
     """ # noqa: E501
-    number: StrictStr
-    hash: StrictStr
-    timestamp: StrictStr
-    __properties: ClassVar[List[str]] = ["number", "hash", "timestamp"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    network: Optional[StrictStr] = None
+    private_key: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["network", "private_key"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Block from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of DogeCoinInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of Block from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of DogeCoinInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "number": obj.get("number"),
-            "hash": obj.get("hash"),
-            "timestamp": obj.get("timestamp")
+            "network": obj.get("network"),
+            "private_key": obj.get("private_key")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/broad_cast_raw_transaction_api_response.py` & `moonsdk-1.0.2/moonsdk/models/tron_api_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from moonsdk.models.broad_cast_raw_transaction_response import BroadCastRawTransactionResponse
 from moonsdk.models.input_body import InputBody
+from moonsdk.models.tron_transaction_output import TronTransactionOutput
 from typing import Optional, Set
 from typing_extensions import Self
 
-class BroadCastRawTransactionAPIResponse(BaseModel):
+class TronAPIResponse(BaseModel):
     """
-    BroadCastRawTransactionAPIResponse
+    TronAPIResponse
     """ # noqa: E501
     success: StrictBool
     message: StrictStr
     body: Optional[InputBody] = None
     address: Optional[StrictStr] = None
-    data: Optional[BroadCastRawTransactionResponse] = None
+    data: Optional[TronTransactionOutput] = None
     __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -49,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of BroadCastRawTransactionAPIResponse from a JSON string"""
+        """Create an instance of TronAPIResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,24 +80,24 @@
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of BroadCastRawTransactionAPIResponse from a dict"""
+        """Create an instance of TronAPIResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "success": obj.get("success"),
             "message": obj.get("message"),
             "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
             "address": obj.get("address"),
-            "data": BroadCastRawTransactionResponse.from_dict(obj["data"]) if obj.get("data") is not None else None
+            "data": TronTransactionOutput.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/broad_cast_raw_transaction_response.py` & `moonsdk-1.0.2/moonsdk/models/broad_cast_raw_transaction_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/broadcast_input.py` & `moonsdk-1.0.2/moonsdk/models/broadcast_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/conveyor_finance_controller_response.py` & `moonsdk-1.0.2/moonsdk/models/conveyor_finance_controller_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/cosmos_api_response.py` & `moonsdk-1.0.2/moonsdk/models/cosmos_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/cosmos_input.py` & `moonsdk-1.0.2/moonsdk/models/cosmos_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/cosmos_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/cosmos_transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/cosmos_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/cosmos_transaction_output.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/create_account_input.py` & `moonsdk-1.0.2/moonsdk/models/create_account_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/create_payment_intent_input.py` & `moonsdk-1.0.2/moonsdk/models/eos_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,84 +13,77 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class CreatePaymentIntentInput(BaseModel):
+class EosInput(BaseModel):
     """
-    CreatePaymentIntentInput
+    EosInput
     """ # noqa: E501
-    config: Optional[StrictStr] = None
-    metadata: Dict[str, StrictStr]
     network: Optional[StrictStr] = None
-    amount: Union[StrictFloat, StrictInt]
-    currency: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["config", "metadata", "network", "amount", "currency"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    private_key: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["network", "private_key"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CreatePaymentIntentInput from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of EosInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of CreatePaymentIntentInput from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of EosInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "config": obj.get("config"),
-            "metadata": obj.get("metadata"),
             "network": obj.get("network"),
-            "amount": obj.get("amount"),
-            "currency": obj.get("currency")
+            "private_key": obj.get("private_key")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/crypto_currency.py` & `moonsdk-1.0.2/moonsdk/models/crypto_currency.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/deploy_input.py` & `moonsdk-1.0.2/moonsdk/models/deploy_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/doge_coin_api_response.py` & `moonsdk-1.0.2/moonsdk/models/doge_coin_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/doge_coin_input.py` & `moonsdk-1.0.2/moonsdk/models/litecoin_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DogeCoinInput(BaseModel):
+class LitecoinInput(BaseModel):
     """
-    DogeCoinInput
+    LitecoinInput
     """ # noqa: E501
     network: Optional[StrictStr] = None
     private_key: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["network", "private_key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DogeCoinInput from a JSON string"""
+        """Create an instance of LitecoinInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,15 +69,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DogeCoinInput from a dict"""
+        """Create an instance of LitecoinInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `moonsdk-1.0.1/moonsdk/models/doge_coin_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/doge_coin_transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/doge_coin_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/doge_coin_transaction_output.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/ens_resolve_api_response.py` & `moonsdk-1.0.2/moonsdk/models/ens_resolve_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/ens_resolve_input.py` & `moonsdk-1.0.2/moonsdk/models/ens_resolve_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/ens_resolve_response.py` & `moonsdk-1.0.2/moonsdk/models/transaction_input_wallet.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class EnsResolveResponse(BaseModel):
+class TransactionInputWallet(BaseModel):
     """
-    EnsResolveResponse
+    TransactionInputWallet
     """ # noqa: E501
     address: StrictStr
     __properties: ClassVar[List[str]] = ["address"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -43,15 +43,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of EnsResolveResponse from a JSON string"""
+        """Create an instance of TransactionInputWallet from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,15 +68,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of EnsResolveResponse from a dict"""
+        """Create an instance of TransactionInputWallet from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `moonsdk-1.0.1/moonsdk/models/ens_reverse_resolve_response.py` & `moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response_message_inner_icons.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,76 +13,81 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from moonsdk.models.get_supported_on_ramps_response_message_inner_icons_png import GetSupportedOnRampsResponseMessageInnerIconsPng
+from typing import Optional, Set
+from typing_extensions import Self
 
-class ENSReverseResolveResponse(BaseModel):
+class GetSupportedOnRampsResponseMessageInnerIcons(BaseModel):
     """
-    ENSReverseResolveResponse
+    GetSupportedOnRampsResponseMessageInnerIcons
     """ # noqa: E501
-    domain: StrictStr
-    __properties: ClassVar[List[str]] = ["domain"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    png: GetSupportedOnRampsResponseMessageInnerIconsPng
+    svg: StrictStr
+    __properties: ClassVar[List[str]] = ["png", "svg"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ENSReverseResolveResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of GetSupportedOnRampsResponseMessageInnerIcons from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of png
+        if self.png:
+            _dict['png'] = self.png.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ENSReverseResolveResponse from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of GetSupportedOnRampsResponseMessageInnerIcons from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "domain": obj.get("domain")
+            "png": GetSupportedOnRampsResponseMessageInnerIconsPng.from_dict(obj["png"]) if obj.get("png") is not None else None,
+            "svg": obj.get("svg")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/eos_api_response.py` & `moonsdk-1.0.2/moonsdk/models/eos_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/eos_input.py` & `moonsdk-1.0.2/moonsdk/models/ripple_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class EosInput(BaseModel):
+class RippleInput(BaseModel):
     """
-    EosInput
+    RippleInput
     """ # noqa: E501
     network: Optional[StrictStr] = None
     private_key: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["network", "private_key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of EosInput from a JSON string"""
+        """Create an instance of RippleInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,15 +69,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of EosInput from a dict"""
+        """Create an instance of RippleInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `moonsdk-1.0.1/moonsdk/models/eos_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/eos_transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/eos_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/eos_transaction_output.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/erc1155_request.py` & `moonsdk-1.0.2/moonsdk/models/erc1155_request.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/erc1155_response.py` & `moonsdk-1.0.2/moonsdk/models/tx.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,22 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from typing import Optional, Set
+from typing_extensions import Self
 
-class Erc1155Response(BaseModel):
+class Tx(BaseModel):
     """
-    Erc1155Response
+    Tx
     """ # noqa: E501
     type: Optional[Union[StrictFloat, StrictInt]] = None
     chain_id: Optional[Union[StrictFloat, StrictInt]] = None
     data: Optional[StrictStr] = None
     gas: Optional[StrictStr] = None
     gas_price: Optional[StrictStr] = None
     gas_tip_cap: Optional[StrictStr] = None
@@ -43,53 +39,53 @@
     to: Optional[StrictStr] = None
     blob_gas: Optional[StrictStr] = None
     blob_gas_fee_cap: Optional[StrictStr] = None
     blob_hashes: Optional[List[StrictStr]] = None
     v: Optional[StrictStr] = None
     r: Optional[StrictStr] = None
     s: Optional[StrictStr] = None
-    balance_of: Optional[StrictStr] = None
-    balance_of_batch: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["type", "chain_id", "data", "gas", "gas_price", "gas_tip_cap", "gas_fee_cap", "value", "nonce", "from", "to", "blob_gas", "blob_gas_fee_cap", "blob_hashes", "v", "r", "s", "balance_of", "balance_of_batch"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    __properties: ClassVar[List[str]] = ["type", "chain_id", "data", "gas", "gas_price", "gas_tip_cap", "gas_fee_cap", "value", "nonce", "from", "to", "blob_gas", "blob_gas_fee_cap", "blob_hashes", "v", "r", "s"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Erc1155Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of Tx from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         # set to None if gas_tip_cap (nullable) is None
         # and model_fields_set contains the field
         if self.gas_tip_cap is None and "gas_tip_cap" in self.model_fields_set:
             _dict['gas_tip_cap'] = None
 
@@ -117,16 +113,16 @@
         # and model_fields_set contains the field
         if self.blob_hashes is None and "blob_hashes" in self.model_fields_set:
             _dict['blob_hashes'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of Erc1155Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of Tx from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
@@ -142,14 +138,12 @@
             "from": obj.get("from"),
             "to": obj.get("to"),
             "blob_gas": obj.get("blob_gas"),
             "blob_gas_fee_cap": obj.get("blob_gas_fee_cap"),
             "blob_hashes": obj.get("blob_hashes"),
             "v": obj.get("v"),
             "r": obj.get("r"),
-            "s": obj.get("s"),
-            "balance_of": obj.get("balance_of"),
-            "balance_of_batch": obj.get("balance_of_batch")
+            "s": obj.get("s")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/erc20_response.py` & `moonsdk-1.0.2/moonsdk/models/token_swap_params.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,153 +13,119 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from typing import Optional, Set
+from typing_extensions import Self
 
-class Erc20Response(BaseModel):
+class TokenSwapParams(BaseModel):
     """
-    Erc20Response
+    TokenSwapParams
     """ # noqa: E501
-    type: Optional[Union[StrictFloat, StrictInt]] = None
-    chain_id: Optional[Union[StrictFloat, StrictInt]] = None
+    to: Optional[StrictStr] = None
     data: Optional[StrictStr] = None
-    gas: Optional[StrictStr] = None
-    gas_price: Optional[StrictStr] = None
-    gas_tip_cap: Optional[StrictStr] = None
-    gas_fee_cap: Optional[StrictStr] = None
+    input: Optional[StrictStr] = None
     value: Optional[StrictStr] = None
-    nonce: Optional[Union[StrictFloat, StrictInt]] = None
-    var_from: Optional[StrictStr] = Field(default=None, alias="from")
-    to: Optional[StrictStr] = None
-    blob_gas: Optional[StrictStr] = None
-    blob_gas_fee_cap: Optional[StrictStr] = None
-    blob_hashes: Optional[List[StrictStr]] = None
-    v: Optional[StrictStr] = None
-    r: Optional[StrictStr] = None
-    s: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    symbol: Optional[StrictStr] = None
-    decimals: Optional[StrictStr] = None
-    total_supply: Optional[StrictStr] = Field(default=None, alias="totalSupply")
+    nonce: Optional[StrictStr] = None
+    gas: Optional[StrictStr] = None
+    gas_price: Optional[StrictStr] = Field(default=None, alias="gasPrice")
+    chain_id: Optional[StrictStr] = None
+    encoding: Optional[StrictStr] = None
+    eoa: Optional[StrictBool] = Field(default=None, alias="EOA")
     contract_address: Optional[StrictStr] = None
-    balance_of: Optional[StrictStr] = Field(default=None, alias="balanceOf")
-    allowance: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["type", "chain_id", "data", "gas", "gas_price", "gas_tip_cap", "gas_fee_cap", "value", "nonce", "from", "to", "blob_gas", "blob_gas_fee_cap", "blob_hashes", "v", "r", "s", "name", "symbol", "decimals", "totalSupply", "contract_address", "balanceOf", "allowance"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    token_id: Optional[StrictStr] = None
+    token_ids: Optional[StrictStr] = None
+    approved: Optional[StrictBool] = None
+    broadcast: Optional[StrictBool] = None
+    token_in: StrictStr = Field(alias="tokenIn")
+    token_out: StrictStr = Field(alias="tokenOut")
+    token_in_decimals: Union[StrictFloat, StrictInt] = Field(alias="tokenInDecimals")
+    token_out_decimals: Union[StrictFloat, StrictInt] = Field(alias="tokenOutDecimals")
+    amount_in: StrictStr = Field(alias="amountIn")
+    slippage: StrictStr
+    recipient: StrictStr
+    referrer: StrictStr
+    __properties: ClassVar[List[str]] = ["to", "data", "input", "value", "nonce", "gas", "gasPrice", "chain_id", "encoding", "EOA", "contract_address", "token_id", "token_ids", "approved", "broadcast", "tokenIn", "tokenOut", "tokenInDecimals", "tokenOutDecimals", "amountIn", "slippage", "recipient", "referrer"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Erc20Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of TokenSwapParams from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if gas_tip_cap (nullable) is None
-        # and model_fields_set contains the field
-        if self.gas_tip_cap is None and "gas_tip_cap" in self.model_fields_set:
-            _dict['gas_tip_cap'] = None
-
-        # set to None if gas_fee_cap (nullable) is None
-        # and model_fields_set contains the field
-        if self.gas_fee_cap is None and "gas_fee_cap" in self.model_fields_set:
-            _dict['gas_fee_cap'] = None
-
-        # set to None if to (nullable) is None
-        # and model_fields_set contains the field
-        if self.to is None and "to" in self.model_fields_set:
-            _dict['to'] = None
-
-        # set to None if blob_gas (nullable) is None
-        # and model_fields_set contains the field
-        if self.blob_gas is None and "blob_gas" in self.model_fields_set:
-            _dict['blob_gas'] = None
-
-        # set to None if blob_gas_fee_cap (nullable) is None
-        # and model_fields_set contains the field
-        if self.blob_gas_fee_cap is None and "blob_gas_fee_cap" in self.model_fields_set:
-            _dict['blob_gas_fee_cap'] = None
-
-        # set to None if blob_hashes (nullable) is None
-        # and model_fields_set contains the field
-        if self.blob_hashes is None and "blob_hashes" in self.model_fields_set:
-            _dict['blob_hashes'] = None
-
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of Erc20Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of TokenSwapParams from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
-            "chain_id": obj.get("chain_id"),
+            "to": obj.get("to"),
             "data": obj.get("data"),
-            "gas": obj.get("gas"),
-            "gas_price": obj.get("gas_price"),
-            "gas_tip_cap": obj.get("gas_tip_cap"),
-            "gas_fee_cap": obj.get("gas_fee_cap"),
+            "input": obj.get("input"),
             "value": obj.get("value"),
             "nonce": obj.get("nonce"),
-            "from": obj.get("from"),
-            "to": obj.get("to"),
-            "blob_gas": obj.get("blob_gas"),
-            "blob_gas_fee_cap": obj.get("blob_gas_fee_cap"),
-            "blob_hashes": obj.get("blob_hashes"),
-            "v": obj.get("v"),
-            "r": obj.get("r"),
-            "s": obj.get("s"),
-            "name": obj.get("name"),
-            "symbol": obj.get("symbol"),
-            "decimals": obj.get("decimals"),
-            "totalSupply": obj.get("totalSupply"),
+            "gas": obj.get("gas"),
+            "gasPrice": obj.get("gasPrice"),
+            "chain_id": obj.get("chain_id"),
+            "encoding": obj.get("encoding"),
+            "EOA": obj.get("EOA"),
             "contract_address": obj.get("contract_address"),
-            "balanceOf": obj.get("balanceOf"),
-            "allowance": obj.get("allowance")
+            "token_id": obj.get("token_id"),
+            "token_ids": obj.get("token_ids"),
+            "approved": obj.get("approved"),
+            "broadcast": obj.get("broadcast"),
+            "tokenIn": obj.get("tokenIn"),
+            "tokenOut": obj.get("tokenOut"),
+            "tokenInDecimals": obj.get("tokenInDecimals"),
+            "tokenOutDecimals": obj.get("tokenOutDecimals"),
+            "amountIn": obj.get("amountIn"),
+            "slippage": obj.get("slippage"),
+            "recipient": obj.get("recipient"),
+            "referrer": obj.get("referrer")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/erc721_request.py` & `moonsdk-1.0.2/moonsdk/models/erc721_request.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/fiat_currency.py` & `moonsdk-1.0.2/moonsdk/models/fiat_currency.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response.py` & `moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response_message_inner.py` & `moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response_message_inner.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response_message_inner_icons.py` & `moonsdk-1.0.2/moonsdk/models/supported_currencies_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from moonsdk.models.get_supported_on_ramps_response_message_inner_icons_png import GetSupportedOnRampsResponseMessageInnerIconsPng
+from moonsdk.models.message import Message
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetSupportedOnRampsResponseMessageInnerIcons(BaseModel):
+class SupportedCurrenciesResponse(BaseModel):
     """
-    GetSupportedOnRampsResponseMessageInnerIcons
+    SupportedCurrenciesResponse
     """ # noqa: E501
-    png: GetSupportedOnRampsResponseMessageInnerIconsPng
-    svg: StrictStr
-    __properties: ClassVar[List[str]] = ["png", "svg"]
+    message: Message
+    __properties: ClassVar[List[str]] = ["message"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetSupportedOnRampsResponseMessageInnerIcons from a JSON string"""
+        """Create an instance of SupportedCurrenciesResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,28 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of png
-        if self.png:
-            _dict['png'] = self.png.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of message
+        if self.message:
+            _dict['message'] = self.message.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetSupportedOnRampsResponseMessageInnerIcons from a dict"""
+        """Create an instance of SupportedCurrenciesResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "png": GetSupportedOnRampsResponseMessageInnerIconsPng.from_dict(obj["png"]) if obj.get("png") is not None else None,
-            "svg": obj.get("svg")
+            "message": Message.from_dict(obj["message"]) if obj.get("message") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/get_supported_on_ramps_response_message_inner_icons_png.py` & `moonsdk-1.0.2/moonsdk/models/get_supported_on_ramps_response_message_inner_icons_png.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/get_swap_dto.py` & `moonsdk-1.0.2/moonsdk/models/get_swap_dto.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/i_native_balance.py` & `moonsdk-1.0.2/moonsdk/models/solana_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,78 +13,77 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class INativeBalance(BaseModel):
+class SolanaInput(BaseModel):
     """
-    INativeBalance
+    SolanaInput
     """ # noqa: E501
-    address: StrictStr
-    balance: StrictStr
-    __properties: ClassVar[List[str]] = ["address", "balance"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    network: Optional[StrictStr] = None
+    private_key: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["network", "private_key"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of INativeBalance from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of SolanaInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of INativeBalance from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of SolanaInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "address": obj.get("address"),
-            "balance": obj.get("balance")
+            "network": obj.get("network"),
+            "private_key": obj.get("private_key")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/i_old_nft_approval.py` & `moonsdk-1.0.2/moonsdk/models/litecoin_api_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,95 +13,91 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from moonsdk.models.input_body import InputBody
+from moonsdk.models.litecoin_transaction_output import LitecoinTransactionOutput
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel
-from pydantic import Field
-from moonsdk.models.inft_approval_erc1155 import INFTApprovalERC1155
-from moonsdk.models.inft_approval_erc721 import INFTApprovalERC721
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class IOldNFTApproval(BaseModel):
+class LitecoinAPIResponse(BaseModel):
     """
-    IOldNFTApproval
+    LitecoinAPIResponse
     """ # noqa: E501
-    erc721: List[INFTApprovalERC721] = Field(alias="ERC721")
-    erc1155: List[INFTApprovalERC1155] = Field(alias="ERC1155")
-    __properties: ClassVar[List[str]] = ["ERC721", "ERC1155"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    success: StrictBool
+    message: StrictStr
+    body: Optional[InputBody] = None
+    address: Optional[StrictStr] = None
+    data: Optional[LitecoinTransactionOutput] = None
+    __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of IOldNFTApproval from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of LitecoinAPIResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in erc721 (list)
-        _items = []
-        if self.erc721:
-            for _item in self.erc721:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['ERC721'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in erc1155 (list)
-        _items = []
-        if self.erc1155:
-            for _item in self.erc1155:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['ERC1155'] = _items
+        # override the default output from pydantic by calling `to_dict()` of body
+        if self.body:
+            _dict['body'] = self.body.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of IOldNFTApproval from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of LitecoinAPIResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "ERC721": [INFTApprovalERC721.from_dict(_item) for _item in obj.get("ERC721")] if obj.get("ERC721") is not None else None,
-            "ERC1155": [INFTApprovalERC1155.from_dict(_item) for _item in obj.get("ERC1155")] if obj.get("ERC1155") is not None else None
+            "success": obj.get("success"),
+            "message": obj.get("message"),
+            "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
+            "address": obj.get("address"),
+            "data": LitecoinTransactionOutput.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/ierc20_approval.py` & `moonsdk-1.0.2/moonsdk/models/transaction_api_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,105 +13,105 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-from moonsdk.models.trigger_output import TriggerOutput
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from moonsdk.models.input_body import InputBody
+from moonsdk.models.transaction import Transaction
+from typing import Optional, Set
+from typing_extensions import Self
 
-class IERC20Approval(BaseModel):
+class TransactionAPIResponse(BaseModel):
     """
-    IERC20Approval
+    TransactionAPIResponse
     """ # noqa: E501
-    transaction_hash: StrictStr = Field(alias="transactionHash")
-    contract: StrictStr
-    log_index: StrictStr = Field(alias="logIndex")
-    owner: StrictStr
-    spender: StrictStr
-    value: StrictStr
-    token_decimals: StrictStr = Field(alias="tokenDecimals")
-    token_name: StrictStr = Field(alias="tokenName")
-    token_symbol: StrictStr = Field(alias="tokenSymbol")
-    value_with_decimals: Optional[StrictStr] = Field(default=None, alias="valueWithDecimals")
-    triggers: Optional[List[TriggerOutput]] = None
-    __properties: ClassVar[List[str]] = ["transactionHash", "contract", "logIndex", "owner", "spender", "value", "tokenDecimals", "tokenName", "tokenSymbol", "valueWithDecimals", "triggers"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    success: StrictBool
+    message: StrictStr
+    body: Optional[InputBody] = None
+    address: Optional[StrictStr] = None
+    transaction_hash: Optional[Any] = None
+    signed_tx: Optional[Any] = Field(default=None, alias="signedTx")
+    data: Optional[Transaction] = None
+    __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "transaction_hash", "signedTx", "data"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of IERC20Approval from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of TransactionAPIResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in triggers (list)
-        _items = []
-        if self.triggers:
-            for _item in self.triggers:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['triggers'] = _items
+        # override the default output from pydantic by calling `to_dict()` of body
+        if self.body:
+            _dict['body'] = self.body.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
+        # set to None if transaction_hash (nullable) is None
+        # and model_fields_set contains the field
+        if self.transaction_hash is None and "transaction_hash" in self.model_fields_set:
+            _dict['transaction_hash'] = None
+
+        # set to None if signed_tx (nullable) is None
+        # and model_fields_set contains the field
+        if self.signed_tx is None and "signed_tx" in self.model_fields_set:
+            _dict['signedTx'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of IERC20Approval from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of TransactionAPIResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "transactionHash": obj.get("transactionHash"),
-            "contract": obj.get("contract"),
-            "logIndex": obj.get("logIndex"),
-            "owner": obj.get("owner"),
-            "spender": obj.get("spender"),
-            "value": obj.get("value"),
-            "tokenDecimals": obj.get("tokenDecimals"),
-            "tokenName": obj.get("tokenName"),
-            "tokenSymbol": obj.get("tokenSymbol"),
-            "valueWithDecimals": obj.get("valueWithDecimals"),
-            "triggers": [TriggerOutput.from_dict(_item) for _item in obj.get("triggers")] if obj.get("triggers") is not None else None
+            "success": obj.get("success"),
+            "message": obj.get("message"),
+            "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
+            "address": obj.get("address"),
+            "transaction_hash": obj.get("transaction_hash"),
+            "signedTx": obj.get("signedTx"),
+            "data": Transaction.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/ierc20_transfer.py` & `moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params_theme.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,105 +13,94 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-from moonsdk.models.trigger_output import TriggerOutput
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class IERC20Transfer(BaseModel):
+class TransactionInputSupportedParamsTheme(BaseModel):
     """
-    IERC20Transfer
+    TransactionInputSupportedParamsTheme
     """ # noqa: E501
-    transaction_hash: StrictStr = Field(alias="transactionHash")
-    contract: StrictStr
-    log_index: StrictStr = Field(alias="logIndex")
-    var_from: StrictStr = Field(alias="from")
-    to: StrictStr
-    value: StrictStr
-    token_decimals: StrictStr = Field(alias="tokenDecimals")
-    token_name: StrictStr = Field(alias="tokenName")
-    token_symbol: StrictStr = Field(alias="tokenSymbol")
-    value_with_decimals: Optional[StrictStr] = Field(default=None, alias="valueWithDecimals")
-    triggers: Optional[List[TriggerOutput]] = None
-    __properties: ClassVar[List[str]] = ["transactionHash", "contract", "logIndex", "from", "to", "value", "tokenDecimals", "tokenName", "tokenSymbol", "valueWithDecimals", "triggers"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    border_radius: Optional[Union[StrictFloat, StrictInt]] = Field(alias="borderRadius")
+    card_color: StrictStr = Field(alias="cardColor")
+    secondary_text_color: StrictStr = Field(alias="secondaryTextColor")
+    primary_text_color: StrictStr = Field(alias="primaryTextColor")
+    secondary_color: StrictStr = Field(alias="secondaryColor")
+    primary_color: StrictStr = Field(alias="primaryColor")
+    theme_name: StrictStr = Field(alias="themeName")
+    is_dark: StrictBool = Field(alias="isDark")
+    __properties: ClassVar[List[str]] = ["borderRadius", "cardColor", "secondaryTextColor", "primaryTextColor", "secondaryColor", "primaryColor", "themeName", "isDark"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of IERC20Transfer from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of TransactionInputSupportedParamsTheme from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in triggers (list)
-        _items = []
-        if self.triggers:
-            for _item in self.triggers:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['triggers'] = _items
+        # set to None if border_radius (nullable) is None
+        # and model_fields_set contains the field
+        if self.border_radius is None and "border_radius" in self.model_fields_set:
+            _dict['borderRadius'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of IERC20Transfer from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of TransactionInputSupportedParamsTheme from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "transactionHash": obj.get("transactionHash"),
-            "contract": obj.get("contract"),
-            "logIndex": obj.get("logIndex"),
-            "from": obj.get("from"),
-            "to": obj.get("to"),
-            "value": obj.get("value"),
-            "tokenDecimals": obj.get("tokenDecimals"),
-            "tokenName": obj.get("tokenName"),
-            "tokenSymbol": obj.get("tokenSymbol"),
-            "valueWithDecimals": obj.get("valueWithDecimals"),
-            "triggers": [TriggerOutput.from_dict(_item) for _item in obj.get("triggers")] if obj.get("triggers") is not None else None
+            "borderRadius": obj.get("borderRadius"),
+            "cardColor": obj.get("cardColor"),
+            "secondaryTextColor": obj.get("secondaryTextColor"),
+            "primaryTextColor": obj.get("primaryTextColor"),
+            "secondaryColor": obj.get("secondaryColor"),
+            "primaryColor": obj.get("primaryColor"),
+            "themeName": obj.get("themeName"),
+            "isDark": obj.get("isDark")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/inft_approval.py` & `moonsdk-1.0.2/moonsdk/models/transaction_response_info.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,100 +13,83 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictBool, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class INFTApproval(BaseModel):
+class TransactionResponseInfo(BaseModel):
     """
-    INFTApproval
+    TransactionResponseInfo
     """ # noqa: E501
-    transaction_hash: StrictStr = Field(alias="transactionHash")
-    contract: StrictStr
-    log_index: StrictStr = Field(alias="logIndex")
-    token_contract_type: StrictStr = Field(alias="tokenContractType")
-    token_name: StrictStr = Field(alias="tokenName")
-    token_symbol: StrictStr = Field(alias="tokenSymbol")
-    account: StrictStr
-    operator: StrictStr
-    approved_all: StrictBool = Field(alias="approvedAll")
-    token_id: Optional[StrictStr] = Field(alias="tokenId")
-    __properties: ClassVar[List[str]] = ["transactionHash", "contract", "logIndex", "tokenContractType", "tokenName", "tokenSymbol", "account", "operator", "approvedAll", "tokenId"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    conveyor_gas: StrictStr = Field(alias="conveyorGas")
+    affiliate_gas: StrictStr = Field(alias="affiliateGas")
+    affiliate_aggregator: StrictStr = Field(alias="affiliateAggregator")
+    amount_out: StrictStr = Field(alias="amountOut")
+    amount_out_min: StrictStr = Field(alias="amountOutMin")
+    __properties: ClassVar[List[str]] = ["conveyorGas", "affiliateGas", "affiliateAggregator", "amountOut", "amountOutMin"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of INFTApproval from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of TransactionResponseInfo from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if token_id (nullable) is None
-        # and model_fields_set contains the field
-        if self.token_id is None and "token_id" in self.model_fields_set:
-            _dict['tokenId'] = None
-
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of INFTApproval from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of TransactionResponseInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "transactionHash": obj.get("transactionHash"),
-            "contract": obj.get("contract"),
-            "logIndex": obj.get("logIndex"),
-            "tokenContractType": obj.get("tokenContractType"),
-            "tokenName": obj.get("tokenName"),
-            "tokenSymbol": obj.get("tokenSymbol"),
-            "account": obj.get("account"),
-            "operator": obj.get("operator"),
-            "approvedAll": obj.get("approvedAll"),
-            "tokenId": obj.get("tokenId")
+            "conveyorGas": obj.get("conveyorGas"),
+            "affiliateGas": obj.get("affiliateGas"),
+            "affiliateAggregator": obj.get("affiliateAggregator"),
+            "amountOut": obj.get("amountOut"),
+            "amountOutMin": obj.get("amountOutMin")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/inft_approval_erc721.py` & `moonsdk-1.0.2/moonsdk/models/ping_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,93 +13,75 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from typing import Optional, Set
+from typing_extensions import Self
 
-class INFTApprovalERC721(BaseModel):
+class PingResponse(BaseModel):
     """
-    INFTApprovalERC721
+    PingResponse
     """ # noqa: E501
-    transaction_hash: StrictStr = Field(alias="transactionHash")
-    contract: StrictStr
-    log_index: StrictStr = Field(alias="logIndex")
-    owner: StrictStr
-    approved: StrictStr
-    token_id: StrictStr = Field(alias="tokenId")
-    token_contract_type: StrictStr = Field(alias="tokenContractType")
-    token_name: StrictStr = Field(alias="tokenName")
-    token_symbol: StrictStr = Field(alias="tokenSymbol")
-    __properties: ClassVar[List[str]] = ["transactionHash", "contract", "logIndex", "owner", "approved", "tokenId", "tokenContractType", "tokenName", "tokenSymbol"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    message: StrictStr
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of INFTApprovalERC721 from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of PingResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of INFTApprovalERC721 from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of PingResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "transactionHash": obj.get("transactionHash"),
-            "contract": obj.get("contract"),
-            "logIndex": obj.get("logIndex"),
-            "owner": obj.get("owner"),
-            "approved": obj.get("approved"),
-            "tokenId": obj.get("tokenId"),
-            "tokenContractType": obj.get("tokenContractType"),
-            "tokenName": obj.get("tokenName"),
-            "tokenSymbol": obj.get("tokenSymbol")
+            "message": obj.get("message")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/input_body.py` & `moonsdk-1.0.2/moonsdk/models/input_body.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/internal_transaction.py` & `moonsdk-1.0.2/moonsdk/models/nonce_api_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,105 +13,91 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from moonsdk.models.input_body import InputBody
+from moonsdk.models.nonce_response import NonceResponse
+from typing import Optional, Set
+from typing_extensions import Self
 
-class InternalTransaction(BaseModel):
+class NonceAPIResponse(BaseModel):
     """
-    InternalTransaction
+    NonceAPIResponse
     """ # noqa: E501
-    var_from: Optional[StrictStr] = Field(alias="from")
-    to: Optional[StrictStr]
-    value: Optional[StrictStr]
-    transaction_hash: StrictStr = Field(alias="transactionHash")
-    gas: Optional[StrictStr]
-    __properties: ClassVar[List[str]] = ["from", "to", "value", "transactionHash", "gas"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    success: StrictBool
+    message: StrictStr
+    body: Optional[InputBody] = None
+    address: Optional[StrictStr] = None
+    data: Optional[NonceResponse] = None
+    __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of InternalTransaction from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of NonceAPIResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if var_from (nullable) is None
-        # and model_fields_set contains the field
-        if self.var_from is None and "var_from" in self.model_fields_set:
-            _dict['from'] = None
-
-        # set to None if to (nullable) is None
-        # and model_fields_set contains the field
-        if self.to is None and "to" in self.model_fields_set:
-            _dict['to'] = None
-
-        # set to None if value (nullable) is None
-        # and model_fields_set contains the field
-        if self.value is None and "value" in self.model_fields_set:
-            _dict['value'] = None
-
-        # set to None if gas (nullable) is None
-        # and model_fields_set contains the field
-        if self.gas is None and "gas" in self.model_fields_set:
-            _dict['gas'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of body
+        if self.body:
+            _dict['body'] = self.body.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of InternalTransaction from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of NonceAPIResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "from": obj.get("from"),
-            "to": obj.get("to"),
-            "value": obj.get("value"),
-            "transactionHash": obj.get("transactionHash"),
-            "gas": obj.get("gas")
+            "success": obj.get("success"),
+            "message": obj.get("message"),
+            "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
+            "address": obj.get("address"),
+            "data": NonceResponse.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/litecoin_api_response.py` & `moonsdk-1.0.2/moonsdk/models/solana_api_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from moonsdk.models.input_body import InputBody
-from moonsdk.models.litecoin_transaction_output import LitecoinTransactionOutput
+from moonsdk.models.solana_transaction_output import SolanaTransactionOutput
 from typing import Optional, Set
 from typing_extensions import Self
 
-class LitecoinAPIResponse(BaseModel):
+class SolanaAPIResponse(BaseModel):
     """
-    LitecoinAPIResponse
+    SolanaAPIResponse
     """ # noqa: E501
     success: StrictBool
     message: StrictStr
     body: Optional[InputBody] = None
     address: Optional[StrictStr] = None
-    data: Optional[LitecoinTransactionOutput] = None
+    data: Optional[SolanaTransactionOutput] = None
     __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -49,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of LitecoinAPIResponse from a JSON string"""
+        """Create an instance of SolanaAPIResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,24 +80,24 @@
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of LitecoinAPIResponse from a dict"""
+        """Create an instance of SolanaAPIResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "success": obj.get("success"),
             "message": obj.get("message"),
             "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
             "address": obj.get("address"),
-            "data": LitecoinTransactionOutput.from_dict(obj["data"]) if obj.get("data") is not None else None
+            "data": SolanaTransactionOutput.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/litecoin_input.py` & `moonsdk-1.0.2/moonsdk/models/tron_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class LitecoinInput(BaseModel):
+class TronInput(BaseModel):
     """
-    LitecoinInput
+    TronInput
     """ # noqa: E501
     network: Optional[StrictStr] = None
     private_key: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["network", "private_key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of LitecoinInput from a JSON string"""
+        """Create an instance of TronInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,15 +69,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of LitecoinInput from a dict"""
+        """Create an instance of TronInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `moonsdk-1.0.1/moonsdk/models/litecoin_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/litecoin_transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/litecoin_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/litecoin_transaction_output.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/message.py` & `moonsdk-1.0.2/moonsdk/models/transaction_response_tx.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
-from typing import Any, ClassVar, Dict, List
-from moonsdk.models.crypto_currency import CryptoCurrency
-from moonsdk.models.fiat_currency import FiatCurrency
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Message(BaseModel):
+class TransactionResponseTx(BaseModel):
     """
-    Message
+    TransactionResponseTx
     """ # noqa: E501
-    fiat: List[FiatCurrency]
-    crypto: List[CryptoCurrency]
-    __properties: ClassVar[List[str]] = ["fiat", "crypto"]
+    data: StrictStr
+    value: StrictStr
+    nonce: Union[StrictFloat, StrictInt]
+    gas: StrictStr
+    to: StrictStr
+    var_from: StrictStr = Field(alias="from")
+    __properties: ClassVar[List[str]] = ["data", "value", "nonce", "gas", "to", "from"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Message from a JSON string"""
+        """Create an instance of TransactionResponseTx from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,39 +69,29 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in fiat (list)
-        _items = []
-        if self.fiat:
-            for _item in self.fiat:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['fiat'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in crypto (list)
-        _items = []
-        if self.crypto:
-            for _item in self.crypto:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['crypto'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Message from a dict"""
+        """Create an instance of TransactionResponseTx from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "fiat": [FiatCurrency.from_dict(_item) for _item in obj["fiat"]] if obj.get("fiat") is not None else None,
-            "crypto": [CryptoCurrency.from_dict(_item) for _item in obj["crypto"]] if obj.get("crypto") is not None else None
+            "data": obj.get("data"),
+            "value": obj.get("value"),
+            "nonce": obj.get("nonce"),
+            "gas": obj.get("gas"),
+            "to": obj.get("to"),
+            "from": obj.get("from")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/nonce_api_response.py` & `moonsdk-1.0.2/moonsdk/models/sign_message_api_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from moonsdk.models.input_body import InputBody
-from moonsdk.models.nonce_response import NonceResponse
+from moonsdk.models.transaction_data import TransactionData
 from typing import Optional, Set
 from typing_extensions import Self
 
-class NonceAPIResponse(BaseModel):
+class SignMessageAPIResponse(BaseModel):
     """
-    NonceAPIResponse
+    SignMessageAPIResponse
     """ # noqa: E501
     success: StrictBool
     message: StrictStr
     body: Optional[InputBody] = None
     address: Optional[StrictStr] = None
-    data: Optional[NonceResponse] = None
+    data: Optional[TransactionData] = None
     __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -49,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of NonceAPIResponse from a JSON string"""
+        """Create an instance of SignMessageAPIResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,24 +80,24 @@
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of NonceAPIResponse from a dict"""
+        """Create an instance of SignMessageAPIResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "success": obj.get("success"),
             "message": obj.get("message"),
             "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
             "address": obj.get("address"),
-            "data": NonceResponse.from_dict(obj["data"]) if obj.get("data") is not None else None
+            "data": TransactionData.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/nonce_response.py` & `moonsdk-1.0.2/moonsdk/models/nonce_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/payment_intent_response.py` & `moonsdk-1.0.2/moonsdk/models/supported_default_response_defaults_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,96 +13,83 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Union
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from pydantic import BaseModel, StrictBool, StrictFloat, StrictInt, StrictStr
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
-
-class PaymentIntentResponse(BaseModel):
+class SupportedDefaultResponseDefaultsId(BaseModel):
     """
-    PaymentIntentResponse
+    SupportedDefaultResponseDefaultsId
     """ # noqa: E501
-    metadata: Optional[Dict[str, StrictStr]] = None
-    uri: Optional[StrictStr] = None
-    qr_code: Optional[StrictStr] = None
-    status: Optional[StrictStr] = None
-    destination: Optional[StrictStr] = None
-    amount: Optional[Union[StrictFloat, StrictInt]] = None
-    network: Optional[StrictStr] = None
-    currency: Optional[StrictStr] = None
-    id: Optional[StrictStr] = None
-    message: Optional[StrictStr] = None
-    success: StrictBool
-    __properties: ClassVar[List[str]] = ["metadata", "uri", "qr_code", "status", "destination", "amount", "network", "currency", "id", "message", "success"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    provider: StrictStr
+    payment_method: StrictStr = Field(alias="paymentMethod")
+    amount: Union[StrictFloat, StrictInt]
+    target: StrictStr
+    source: StrictStr
+    __properties: ClassVar[List[str]] = ["provider", "paymentMethod", "amount", "target", "source"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaymentIntentResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of SupportedDefaultResponseDefaultsId from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaymentIntentResponse from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of SupportedDefaultResponseDefaultsId from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "metadata": obj.get("metadata"),
-            "uri": obj.get("uri"),
-            "qr_code": obj.get("qr_code"),
-            "status": obj.get("status"),
-            "destination": obj.get("destination"),
+            "provider": obj.get("provider"),
+            "paymentMethod": obj.get("paymentMethod"),
             "amount": obj.get("amount"),
-            "network": obj.get("network"),
-            "currency": obj.get("currency"),
-            "id": obj.get("id"),
-            "message": obj.get("message"),
-            "success": obj.get("success")
+            "target": obj.get("target"),
+            "source": obj.get("source")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/payment_type.py` & `moonsdk-1.0.2/moonsdk/models/payment_type.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/ping_response.py` & `moonsdk-1.0.2/moonsdk/models/supported_asset_response_assets_inner.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PingResponse(BaseModel):
+class SupportedAssetResponseAssetsInner(BaseModel):
     """
-    PingResponse
+    SupportedAssetResponseAssetsInner
     """ # noqa: E501
-    message: StrictStr
-    __properties: ClassVar[List[str]] = ["message"]
+    crypto: List[StrictStr]
+    payment_methods: List[StrictStr] = Field(alias="paymentMethods")
+    fiat: StrictStr
+    __properties: ClassVar[List[str]] = ["crypto", "paymentMethods", "fiat"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -43,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PingResponse from a JSON string"""
+        """Create an instance of SupportedAssetResponseAssetsInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,20 +70,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PingResponse from a dict"""
+        """Create an instance of SupportedAssetResponseAssetsInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "message": obj.get("message")
+            "crypto": obj.get("crypto"),
+            "paymentMethods": obj.get("paymentMethods"),
+            "fiat": obj.get("fiat")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/quote.py` & `moonsdk-1.0.2/moonsdk/models/quote.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/ripple_api_response.py` & `moonsdk-1.0.2/moonsdk/models/ripple_api_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/ripple_input.py` & `moonsdk-1.0.2/moonsdk/models/solana_transaction_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RippleInput(BaseModel):
+class SolanaTransactionInput(BaseModel):
     """
-    RippleInput
+    SolanaTransactionInput
     """ # noqa: E501
+    to: Optional[StrictStr] = None
+    value: Optional[Union[StrictFloat, StrictInt]] = None
     network: Optional[StrictStr] = None
-    private_key: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["network", "private_key"]
+    compress: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["to", "value", "network", "compress"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RippleInput from a JSON string"""
+        """Create an instance of SolanaTransactionInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,21 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RippleInput from a dict"""
+        """Create an instance of SolanaTransactionInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "to": obj.get("to"),
+            "value": obj.get("value"),
             "network": obj.get("network"),
-            "private_key": obj.get("private_key")
+            "compress": obj.get("compress")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/ripple_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/ripple_transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/ripple_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/ripple_transaction_output.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/sell_quote.py` & `moonsdk-1.0.2/moonsdk/models/sell_quote.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/sign_message.py` & `moonsdk-1.0.2/moonsdk/models/sign_message.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/sign_message_api_response.py` & `moonsdk-1.0.2/moonsdk/models/supported_asset_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,31 +13,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from moonsdk.models.input_body import InputBody
-from moonsdk.models.transaction_data import TransactionData
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List
+from moonsdk.models.supported_asset_response_assets_inner import SupportedAssetResponseAssetsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SignMessageAPIResponse(BaseModel):
+class SupportedAssetResponse(BaseModel):
     """
-    SignMessageAPIResponse
+    SupportedAssetResponse
     """ # noqa: E501
-    success: StrictBool
-    message: StrictStr
-    body: Optional[InputBody] = None
-    address: Optional[StrictStr] = None
-    data: Optional[TransactionData] = None
-    __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
+    country: StrictStr
+    assets: List[SupportedAssetResponseAssetsInner]
+    __properties: ClassVar[List[str]] = ["country", "assets"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SignMessageAPIResponse from a JSON string"""
+        """Create an instance of SupportedAssetResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,34 +66,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of body
-        if self.body:
-            _dict['body'] = self.body.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of data
-        if self.data:
-            _dict['data'] = self.data.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in assets (list)
+        _items = []
+        if self.assets:
+            for _item in self.assets:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['assets'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SignMessageAPIResponse from a dict"""
+        """Create an instance of SupportedAssetResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "success": obj.get("success"),
-            "message": obj.get("message"),
-            "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
-            "address": obj.get("address"),
-            "data": TransactionData.from_dict(obj["data"]) if obj.get("data") is not None else None
+            "country": obj.get("country"),
+            "assets": [SupportedAssetResponseAssetsInner.from_dict(_item) for _item in obj["assets"]] if obj.get("assets") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/sign_typed_data.py` & `moonsdk-1.0.2/moonsdk/models/solana_transaction_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SignTypedData(BaseModel):
+class SolanaTransactionOutput(BaseModel):
     """
-    SignTypedData
+    SolanaTransactionOutput
     """ # noqa: E501
-    data: StrictStr
-    __properties: ClassVar[List[str]] = ["data"]
+    signed_tx: Optional[StrictStr] = Field(default=None, alias="signedTx")
+    transaction_hash: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["signedTx", "transaction_hash"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -43,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SignTypedData from a JSON string"""
+        """Create an instance of SolanaTransactionOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,20 +69,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SignTypedData from a dict"""
+        """Create an instance of SolanaTransactionOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "data": obj.get("data")
+            "signedTx": obj.get("signedTx"),
+            "transaction_hash": obj.get("transaction_hash")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/solana_api_response.py` & `moonsdk-1.0.2/moonsdk/models/supported_default_response_defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from moonsdk.models.input_body import InputBody
-from moonsdk.models.solana_transaction_output import SolanaTransactionOutput
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List
+from moonsdk.models.supported_default_response_defaults_id import SupportedDefaultResponseDefaultsId
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SolanaAPIResponse(BaseModel):
+class SupportedDefaultResponseDefaults(BaseModel):
     """
-    SolanaAPIResponse
+    SupportedDefaultResponseDefaults
     """ # noqa: E501
-    success: StrictBool
-    message: StrictStr
-    body: Optional[InputBody] = None
-    address: Optional[StrictStr] = None
-    data: Optional[SolanaTransactionOutput] = None
-    __properties: ClassVar[List[str]] = ["success", "message", "body", "address", "data"]
+    id: SupportedDefaultResponseDefaultsId
+    __properties: ClassVar[List[str]] = ["id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SolanaAPIResponse from a JSON string"""
+        """Create an instance of SupportedDefaultResponseDefaults from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,34 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of body
-        if self.body:
-            _dict['body'] = self.body.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of data
-        if self.data:
-            _dict['data'] = self.data.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of id
+        if self.id:
+            _dict['id'] = self.id.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SolanaAPIResponse from a dict"""
+        """Create an instance of SupportedDefaultResponseDefaults from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "success": obj.get("success"),
-            "message": obj.get("message"),
-            "body": InputBody.from_dict(obj["body"]) if obj.get("body") is not None else None,
-            "address": obj.get("address"),
-            "data": SolanaTransactionOutput.from_dict(obj["data"]) if obj.get("data") is not None else None
+            "id": SupportedDefaultResponseDefaultsId.from_dict(obj["id"]) if obj.get("id") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/solana_input.py` & `moonsdk-1.0.2/moonsdk/models/transaction_input_meta_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SolanaInput(BaseModel):
+class TransactionInputMetaData(BaseModel):
     """
-    SolanaInput
+    TransactionInputMetaData
     """ # noqa: E501
-    network: Optional[StrictStr] = None
-    private_key: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["network", "private_key"]
+    quote_id: StrictStr = Field(alias="quoteId")
+    __properties: ClassVar[List[str]] = ["quoteId"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +43,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SolanaInput from a JSON string"""
+        """Create an instance of TransactionInputMetaData from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,21 +68,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SolanaInput from a dict"""
+        """Create an instance of TransactionInputMetaData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "network": obj.get("network"),
-            "private_key": obj.get("private_key")
+            "quoteId": obj.get("quoteId")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/solana_transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/tron_transaction_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SolanaTransactionInput(BaseModel):
+class TronTransactionInput(BaseModel):
     """
-    SolanaTransactionInput
+    TronTransactionInput
     """ # noqa: E501
     to: Optional[StrictStr] = None
     value: Optional[Union[StrictFloat, StrictInt]] = None
     network: Optional[StrictStr] = None
     compress: Optional[StrictBool] = None
     __properties: ClassVar[List[str]] = ["to", "value", "network", "compress"]
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SolanaTransactionInput from a JSON string"""
+        """Create an instance of TronTransactionInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,15 +71,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SolanaTransactionInput from a dict"""
+        """Create an instance of TronTransactionInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `moonsdk-1.0.1/moonsdk/models/solana_transaction_output.py` & `moonsdk-1.0.2/moonsdk/models/tron_transaction_output.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SolanaTransactionOutput(BaseModel):
+class TronTransactionOutput(BaseModel):
     """
-    SolanaTransactionOutput
+    TronTransactionOutput
     """ # noqa: E501
     signed_tx: Optional[StrictStr] = Field(default=None, alias="signedTx")
     transaction_hash: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["signedTx", "transaction_hash"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SolanaTransactionOutput from a JSON string"""
+        """Create an instance of TronTransactionOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,15 +69,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SolanaTransactionOutput from a dict"""
+        """Create an instance of TronTransactionOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_asset_response.py` & `moonsdk-1.0.2/moonsdk/models/supported_payment_types_currency_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,27 +13,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from moonsdk.models.supported_asset_response_assets_inner import SupportedAssetResponseAssetsInner
+from moonsdk.models.supported_payment_types_message import SupportedPaymentTypesMessage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SupportedAssetResponse(BaseModel):
+class SupportedPaymentTypesCurrencyResponse(BaseModel):
     """
-    SupportedAssetResponse
+    SupportedPaymentTypesCurrencyResponse
     """ # noqa: E501
-    country: StrictStr
-    assets: List[SupportedAssetResponseAssetsInner]
-    __properties: ClassVar[List[str]] = ["country", "assets"]
+    message: SupportedPaymentTypesMessage
+    __properties: ClassVar[List[str]] = ["message"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SupportedAssetResponse from a JSON string"""
+        """Create an instance of SupportedPaymentTypesCurrencyResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,32 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in assets (list)
-        _items = []
-        if self.assets:
-            for _item in self.assets:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['assets'] = _items
+        # override the default output from pydantic by calling `to_dict()` of message
+        if self.message:
+            _dict['message'] = self.message.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SupportedAssetResponse from a dict"""
+        """Create an instance of SupportedPaymentTypesCurrencyResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "country": obj.get("country"),
-            "assets": [SupportedAssetResponseAssetsInner.from_dict(_item) for _item in obj["assets"]] if obj.get("assets") is not None else None
+            "message": SupportedPaymentTypesMessage.from_dict(obj["message"]) if obj.get("message") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_asset_response_assets_inner.py` & `moonsdk-1.0.2/moonsdk/models/transaction_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,27 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Union
+from moonsdk.models.transaction_response_info import TransactionResponseInfo
+from moonsdk.models.transaction_response_tx import TransactionResponseTx
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SupportedAssetResponseAssetsInner(BaseModel):
+class TransactionResponse(BaseModel):
     """
-    SupportedAssetResponseAssetsInner
+    TransactionResponse
     """ # noqa: E501
-    crypto: List[StrictStr]
-    payment_methods: List[StrictStr] = Field(alias="paymentMethods")
-    fiat: StrictStr
-    __properties: ClassVar[List[str]] = ["crypto", "paymentMethods", "fiat"]
+    message: StrictStr
+    tx: TransactionResponseTx
+    info: TransactionResponseInfo
+    chain_id: Union[StrictFloat, StrictInt] = Field(alias="chainId")
+    current_block_number: Union[StrictFloat, StrictInt] = Field(alias="currentBlockNumber")
+    __properties: ClassVar[List[str]] = ["message", "tx", "info", "chainId", "currentBlockNumber"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SupportedAssetResponseAssetsInner from a JSON string"""
+        """Create an instance of TransactionResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,26 +70,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of tx
+        if self.tx:
+            _dict['tx'] = self.tx.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of info
+        if self.info:
+            _dict['info'] = self.info.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SupportedAssetResponseAssetsInner from a dict"""
+        """Create an instance of TransactionResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "crypto": obj.get("crypto"),
-            "paymentMethods": obj.get("paymentMethods"),
-            "fiat": obj.get("fiat")
+            "message": obj.get("message"),
+            "tx": TransactionResponseTx.from_dict(obj["tx"]) if obj.get("tx") is not None else None,
+            "info": TransactionResponseInfo.from_dict(obj["info"]) if obj.get("info") is not None else None,
+            "chainId": obj.get("chainId"),
+            "currentBlockNumber": obj.get("currentBlockNumber")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_currencies_response.py` & `moonsdk-1.0.2/moonsdk/models/transaction_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,26 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
-from typing import Any, ClassVar, Dict, List
-from moonsdk.models.message import Message
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SupportedCurrenciesResponse(BaseModel):
+class TransactionRequest(BaseModel):
     """
-    SupportedCurrenciesResponse
+    TransactionRequest
     """ # noqa: E501
-    message: Message
-    __properties: ClassVar[List[str]] = ["message"]
+    nonce: Optional[StrictStr] = None
+    data: Optional[StrictStr] = None
+    value: Optional[StrictStr] = None
+    to: Optional[StrictStr] = None
+    var_from: Optional[StrictStr] = Field(default=None, alias="from")
+    max_fee_per_gas: Optional[StrictStr] = Field(default=None, alias="maxFeePerGas")
+    max_priority_fee_per_gas: Optional[StrictStr] = Field(default=None, alias="maxPriorityFeePerGas")
+    __properties: ClassVar[List[str]] = ["nonce", "data", "value", "to", "from", "maxFeePerGas", "maxPriorityFeePerGas"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SupportedCurrenciesResponse from a JSON string"""
+        """Create an instance of TransactionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,27 +70,30 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of message
-        if self.message:
-            _dict['message'] = self.message.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SupportedCurrenciesResponse from a dict"""
+        """Create an instance of TransactionRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "message": Message.from_dict(obj["message"]) if obj.get("message") is not None else None
+            "nonce": obj.get("nonce"),
+            "data": obj.get("data"),
+            "value": obj.get("value"),
+            "to": obj.get("to"),
+            "from": obj.get("from"),
+            "maxFeePerGas": obj.get("maxFeePerGas"),
+            "maxPriorityFeePerGas": obj.get("maxPriorityFeePerGas")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_default_response.py` & `moonsdk-1.0.2/moonsdk/models/supported_default_response.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_default_response_defaults.py` & `moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params_partner_data_redirect_url.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from moonsdk.models.supported_default_response_defaults_id import SupportedDefaultResponseDefaultsId
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SupportedDefaultResponseDefaults(BaseModel):
+class TransactionInputSupportedParamsPartnerDataRedirectUrl(BaseModel):
     """
-    SupportedDefaultResponseDefaults
+    TransactionInputSupportedParamsPartnerDataRedirectUrl
     """ # noqa: E501
-    id: SupportedDefaultResponseDefaultsId
-    __properties: ClassVar[List[str]] = ["id"]
+    success: StrictStr
+    __properties: ClassVar[List[str]] = ["success"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +43,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SupportedDefaultResponseDefaults from a JSON string"""
+        """Create an instance of TransactionInputSupportedParamsPartnerDataRedirectUrl from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,27 +64,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of id
-        if self.id:
-            _dict['id'] = self.id.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SupportedDefaultResponseDefaults from a dict"""
+        """Create an instance of TransactionInputSupportedParamsPartnerDataRedirectUrl from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": SupportedDefaultResponseDefaultsId.from_dict(obj["id"]) if obj.get("id") is not None else None
+            "success": obj.get("success")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_default_response_defaults_id.py` & `moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params_partner_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,29 +13,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Union
+from pydantic import BaseModel, ConfigDict, Field
+from typing import Any, ClassVar, Dict, List
+from moonsdk.models.transaction_input_supported_params_partner_data_redirect_url import TransactionInputSupportedParamsPartnerDataRedirectUrl
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SupportedDefaultResponseDefaultsId(BaseModel):
+class TransactionInputSupportedParamsPartnerData(BaseModel):
     """
-    SupportedDefaultResponseDefaultsId
+    TransactionInputSupportedParamsPartnerData
     """ # noqa: E501
-    provider: StrictStr
-    payment_method: StrictStr = Field(alias="paymentMethod")
-    amount: Union[StrictFloat, StrictInt]
-    target: StrictStr
-    source: StrictStr
-    __properties: ClassVar[List[str]] = ["provider", "paymentMethod", "amount", "target", "source"]
+    redirect_url: TransactionInputSupportedParamsPartnerDataRedirectUrl = Field(alias="redirectUrl")
+    __properties: ClassVar[List[str]] = ["redirectUrl"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SupportedDefaultResponseDefaultsId from a JSON string"""
+        """Create an instance of TransactionInputSupportedParamsPartnerData from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,28 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of redirect_url
+        if self.redirect_url:
+            _dict['redirectUrl'] = self.redirect_url.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SupportedDefaultResponseDefaultsId from a dict"""
+        """Create an instance of TransactionInputSupportedParamsPartnerData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "provider": obj.get("provider"),
-            "paymentMethod": obj.get("paymentMethod"),
-            "amount": obj.get("amount"),
-            "target": obj.get("target"),
-            "source": obj.get("source")
+            "redirectUrl": TransactionInputSupportedParamsPartnerDataRedirectUrl.from_dict(obj["redirectUrl"]) if obj.get("redirectUrl") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_payment_types_currency_response.py` & `moonsdk-1.0.2/moonsdk/models/supported_payment_types_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from moonsdk.models.supported_payment_types_message import SupportedPaymentTypesMessage
+from moonsdk.models.payment_type import PaymentType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SupportedPaymentTypesCurrencyResponse(BaseModel):
+class SupportedPaymentTypesMessage(BaseModel):
     """
-    SupportedPaymentTypesCurrencyResponse
+    SupportedPaymentTypesMessage
     """ # noqa: E501
-    message: SupportedPaymentTypesMessage
-    __properties: ClassVar[List[str]] = ["message"]
+    googlepay: PaymentType
+    applepay: PaymentType
+    creditcard: PaymentType
+    __properties: ClassVar[List[str]] = ["googlepay", "applepay", "creditcard"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SupportedPaymentTypesCurrencyResponse from a JSON string"""
+        """Create an instance of SupportedPaymentTypesMessage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,27 +67,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of message
-        if self.message:
-            _dict['message'] = self.message.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of googlepay
+        if self.googlepay:
+            _dict['googlepay'] = self.googlepay.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of applepay
+        if self.applepay:
+            _dict['applepay'] = self.applepay.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of creditcard
+        if self.creditcard:
+            _dict['creditcard'] = self.creditcard.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SupportedPaymentTypesCurrencyResponse from a dict"""
+        """Create an instance of SupportedPaymentTypesMessage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "message": SupportedPaymentTypesMessage.from_dict(obj["message"]) if obj.get("message") is not None else None
+            "googlepay": PaymentType.from_dict(obj["googlepay"]) if obj.get("googlepay") is not None else None,
+            "applepay": PaymentType.from_dict(obj["applepay"]) if obj.get("applepay") is not None else None,
+            "creditcard": PaymentType.from_dict(obj["creditcard"]) if obj.get("creditcard") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/supported_payment_types_message.py` & `moonsdk-1.0.2/moonsdk/models/transaction_input_supported_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
-from moonsdk.models.payment_type import PaymentType
+from moonsdk.models.transaction_input_supported_params_partner_data import TransactionInputSupportedParamsPartnerData
+from moonsdk.models.transaction_input_supported_params_theme import TransactionInputSupportedParamsTheme
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SupportedPaymentTypesMessage(BaseModel):
+class TransactionInputSupportedParams(BaseModel):
     """
-    SupportedPaymentTypesMessage
+    TransactionInputSupportedParams
     """ # noqa: E501
-    googlepay: PaymentType
-    applepay: PaymentType
-    creditcard: PaymentType
-    __properties: ClassVar[List[str]] = ["googlepay", "applepay", "creditcard"]
+    partner_data: TransactionInputSupportedParamsPartnerData = Field(alias="partnerData")
+    theme: TransactionInputSupportedParamsTheme
+    __properties: ClassVar[List[str]] = ["partnerData", "theme"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SupportedPaymentTypesMessage from a JSON string"""
+        """Create an instance of TransactionInputSupportedParams from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,35 +67,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of googlepay
-        if self.googlepay:
-            _dict['googlepay'] = self.googlepay.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of applepay
-        if self.applepay:
-            _dict['applepay'] = self.applepay.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of creditcard
-        if self.creditcard:
-            _dict['creditcard'] = self.creditcard.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of partner_data
+        if self.partner_data:
+            _dict['partnerData'] = self.partner_data.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of theme
+        if self.theme:
+            _dict['theme'] = self.theme.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SupportedPaymentTypesMessage from a dict"""
+        """Create an instance of TransactionInputSupportedParams from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "googlepay": PaymentType.from_dict(obj["googlepay"]) if obj.get("googlepay") is not None else None,
-            "applepay": PaymentType.from_dict(obj["applepay"]) if obj.get("applepay") is not None else None,
-            "creditcard": PaymentType.from_dict(obj["creditcard"]) if obj.get("creditcard") is not None else None
+            "partnerData": TransactionInputSupportedParamsPartnerData.from_dict(obj["partnerData"]) if obj.get("partnerData") is not None else None,
+            "theme": TransactionInputSupportedParamsTheme.from_dict(obj["theme"]) if obj.get("theme") is not None else None
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/token_swap_params.py` & `moonsdk-1.0.2/moonsdk/models/uniswap_input.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TokenSwapParams(BaseModel):
+class UniswapInput(BaseModel):
     """
-    TokenSwapParams
+    UniswapInput
     """ # noqa: E501
     to: Optional[StrictStr] = None
     data: Optional[StrictStr] = None
     input: Optional[StrictStr] = None
     value: Optional[StrictStr] = None
     nonce: Optional[StrictStr] = None
     gas: Optional[StrictStr] = None
@@ -37,23 +37,19 @@
     encoding: Optional[StrictStr] = None
     eoa: Optional[StrictBool] = Field(default=None, alias="EOA")
     contract_address: Optional[StrictStr] = None
     token_id: Optional[StrictStr] = None
     token_ids: Optional[StrictStr] = None
     approved: Optional[StrictBool] = None
     broadcast: Optional[StrictBool] = None
-    token_in: StrictStr = Field(alias="tokenIn")
-    token_out: StrictStr = Field(alias="tokenOut")
-    token_in_decimals: Union[StrictFloat, StrictInt] = Field(alias="tokenInDecimals")
-    token_out_decimals: Union[StrictFloat, StrictInt] = Field(alias="tokenOutDecimals")
-    amount_in: StrictStr = Field(alias="amountIn")
-    slippage: StrictStr
-    recipient: StrictStr
-    referrer: StrictStr
-    __properties: ClassVar[List[str]] = ["to", "data", "input", "value", "nonce", "gas", "gasPrice", "chain_id", "encoding", "EOA", "contract_address", "token_id", "token_ids", "approved", "broadcast", "tokenIn", "tokenOut", "tokenInDecimals", "tokenOutDecimals", "amountIn", "slippage", "recipient", "referrer"]
+    token_a: Optional[StrictStr] = None
+    token_b: Optional[StrictStr] = None
+    amount_a: Optional[StrictStr] = None
+    amount_b: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["to", "data", "input", "value", "nonce", "gas", "gasPrice", "chain_id", "encoding", "EOA", "contract_address", "token_id", "token_ids", "approved", "broadcast", "token_a", "token_b", "amount_a", "amount_b"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -65,15 +61,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TokenSwapParams from a JSON string"""
+        """Create an instance of UniswapInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,15 +86,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TokenSwapParams from a dict"""
+        """Create an instance of UniswapInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
@@ -113,19 +109,15 @@
             "encoding": obj.get("encoding"),
             "EOA": obj.get("EOA"),
             "contract_address": obj.get("contract_address"),
             "token_id": obj.get("token_id"),
             "token_ids": obj.get("token_ids"),
             "approved": obj.get("approved"),
             "broadcast": obj.get("broadcast"),
-            "tokenIn": obj.get("tokenIn"),
-            "tokenOut": obj.get("tokenOut"),
-            "tokenInDecimals": obj.get("tokenInDecimals"),
-            "tokenOutDecimals": obj.get("tokenOutDecimals"),
-            "amountIn": obj.get("amountIn"),
-            "slippage": obj.get("slippage"),
-            "recipient": obj.get("recipient"),
-            "referrer": obj.get("referrer")
+            "token_a": obj.get("token_a"),
+            "token_b": obj.get("token_b"),
+            "amount_a": obj.get("amount_a"),
+            "amount_b": obj.get("amount_b")
         })
         return _obj
```

### Comparing `moonsdk-1.0.1/moonsdk/models/transaction.py` & `moonsdk-1.0.2/moonsdk/models/transaction.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/transaction_data.py` & `moonsdk-1.0.2/moonsdk/models/transaction_data.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/models/transaction_input.py` & `moonsdk-1.0.2/moonsdk/models/transaction_input.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/moonsdk/rest.py` & `moonsdk-1.0.2/moonsdk/rest.py`

 * *Files identical despite different names*

### Comparing `moonsdk-1.0.1/pyproject.toml` & `moonsdk-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moonsdk"
-version = "1.0.1"
+version = "1.0.2"
 description = "moon-vault-api"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/moon-up/moon-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "moon-vault-api"]
 include = ["moonsdk/py.typed"]
```

### Comparing `moonsdk-1.0.1/PKG-INFO` & `moonsdk-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonsdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: moon-vault-api
 Home-page: https://github.com/moon-up/moon-sdk-python
 License: ISC
 Keywords: OpenAPI,OpenAPI-Generator,moon-vault-api
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -41,17 +41,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install moonsdk 
+pip install git+https://github.com/moon-up/moon-sdk-python.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install moonsdk`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/moon-up/moon-sdk-python.git`)
 
 Then import the package:
 ```python
 import moonsdk
 ```
 
 ### Setuptools
```

