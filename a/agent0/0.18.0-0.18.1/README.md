# Comparing `tmp/agent0-0.18.0.tar.gz` & `tmp/agent0-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent0-0.18.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "agent0-0.18.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `agent0-0.18.0.tar` & `agent0-0.18.1.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0     4888 2024-04-15 18:11:44.224159 agent0-0.18.0/README.md
--rw-r--r--   0        0        0     4223 2024-04-15 18:11:44.240159 agent0-0.18.0/pyproject.toml
--rw-r--r--   0        0        0      463 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/__init__.py
--rw-r--r--   0        0        0       87 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/__init__.py
--rw-r--r--   0        0        0      265 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/analysis/__init__.py
--rw-r--r--   0        0        0      876 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/analysis/calc_base_buffer.py
--rw-r--r--   0        0        0     1130 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/analysis/calc_fixed_rate.py
--rw-r--r--   0        0        0     5570 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/analysis/calc_pnl.py
--rw-r--r--   0        0        0     1564 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/analysis/calc_spot_price.py
--rw-r--r--   0        0        0     2140 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/analysis/calc_ticker.py
--rw-r--r--   0        0        0    10619 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/analysis/data_to_analysis.py
--rw-r--r--   0        0        0      581 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/__init__.py
--rw-r--r--   0        0        0      620 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/build_fixed_rate.py
--rw-r--r--   0        0        0     1608 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/build_leaderboard.py
--rw-r--r--   0        0        0     1268 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/build_ohlcv.py
--rw-r--r--   0        0        0      546 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/build_outstanding_positions.py
--rw-r--r--   0        0        0     1250 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/build_ticker.py
--rw-r--r--   0        0        0      720 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/build_variable_rate.py
--rw-r--r--   0        0        0     1038 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/plot_fixed_rate.py
--rw-r--r--   0        0        0      858 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/plot_ohlcv.py
--rw-r--r--   0        0        0      851 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/plot_outstanding_positions.py
--rw-r--r--   0        0        0     1117 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/plot_utils.py
--rw-r--r--   0        0        0     4630 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/dashboard/usernames.py
--rw-r--r--   0        0        0        0 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/db/__init__.py
--rw-r--r--   0        0        0      140 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/db/api/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/db/api/api_interface.py
--rw-r--r--   0        0        0     4334 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/db/api/api_server.py
--rw-r--r--   0        0        0      388 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/db/base/__init__.py
--rw-r--r--   0        0        0    12480 2024-04-15 18:11:44.240159 agent0-0.18.0/src/agent0/chainsync/db/base/interface.py
--rw-r--r--   0        0        0    10937 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/base/interface_test.py
--rw-r--r--   0        0        0     1648 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/base/schema.py
--rw-r--r--   0        0        0     2742 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/base/schema_test.py
--rw-r--r--   0        0        0     1084 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/__init__.py
--rw-r--r--   0        0        0     4303 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/chain_to_db.py
--rw-r--r--   0        0        0    21417 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/convert_data.py
--rw-r--r--   0        0        0     8207 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/import_export_data.py
--rw-r--r--   0        0        0     1218 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/import_export_data_test.py
--rw-r--r--   0        0        0    30568 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/interface.py
--rw-r--r--   0        0        0    21353 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/interface_test.py
--rw-r--r--   0        0        0    15387 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/schema.py
--rw-r--r--   0        0        0     8085 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/schema_test.py
--rw-r--r--   0        0        0      121 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/exec/__init__.py
--rw-r--r--   0        0        0     5884 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/exec/acquire_data.py
--rw-r--r--   0        0        0     6210 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/exec/data_analysis.py
--rw-r--r--   0        0        0     1919 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/postgres_config.py
--rw-r--r--   0        0        0     4066 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/streamlit/Dashboard.py
--rw-r--r--   0        0        0     7174 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/streamlit/pages/Wallet_Stats.py
--rw-r--r--   0        0        0      149 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/test_fixtures/__init__.py
--rw-r--r--   0        0        0     6763 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/test_fixtures/db_session.py
--rw-r--r--   0        0        0     1265 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/chainsync/test_fixtures/dummy_session.py
--rw-r--r--   0        0        0      218 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/__init__.py
--rw-r--r--   0        0        0     8781 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/accounts_config.py
--rw-r--r--   0        0        0      215 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/__init__.py
--rw-r--r--   0        0        0      166 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/agent/__init__.py
--rw-r--r--   0        0        0     3881 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/agent/eth_agent.py
--rw-r--r--   0        0        0     4839 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/agent/eth_wallet.py
--rw-r--r--   0        0        0      954 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/agent/eth_wallet_test.py
--rw-r--r--   0        0        0      414 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/agent/market_actions.py
--rw-r--r--   0        0        0      174 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/config/__init__.py
--rw-r--r--   0        0        0     1237 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/config/agent_config.py
--rw-r--r--   0        0        0     1513 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/config/budget.py
--rw-r--r--   0        0        0     4628 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/config/environment_config.py
--rw-r--r--   0        0        0      747 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/make_key.py
--rw-r--r--   0        0        0      152 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/policies/__init__.py
--rw-r--r--   0        0        0     3407 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/policies/base.py
--rw-r--r--   0        0        0     1368 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/policies/no_action.py
--rw-r--r--   0        0        0     6101 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/types.py
--rw-r--r--   0        0        0     7199 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/base/types_test.py
--rw-r--r--   0        0        0      290 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/__init__.py
--rw-r--r--   0        0        0      606 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/agent/__init__.py
--rw-r--r--   0        0        0     8046 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/agent/build_wallet_positions.py
--rw-r--r--   0        0        0    10266 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_actions.py
--rw-r--r--   0        0        0     5425 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_agent.py
--rw-r--r--   0        0        0     7871 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_wallet.py
--rw-r--r--   0        0        0     2300 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_wallet_test.py
--rw-r--r--   0        0        0     2976 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/agent/trade_result.py
--rw-r--r--   0        0        0      326 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/crash_report/__init__.py
--rw-r--r--   0        0        0    17230 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/crash_report/crash_report.py
--rw-r--r--   0        0        0     9805 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/crash_report/known_error_checks.py
--rw-r--r--   0        0        0      184 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/econ_tests.py
--rw-r--r--   0        0        0     6061 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/event_types.py
--rw-r--r--   0        0        0      241 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/exec/__init__.py
--rw-r--r--   0        0        0     2418 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/exec/check_for_new_block.py
--rw-r--r--   0        0        0    17618 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/exec/execute_agent_trades.py
--rw-r--r--   0        0        0     1284 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/exec/set_max_approval.py
--rw-r--r--   0        0        0     1346 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_chain.py
--rw-r--r--   0        0        0    23041 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_hyperdrive.py
--rw-r--r--   0        0        0     8207 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_hyperdrive_agent.py
--rw-r--r--   0        0        0    16478 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_hyperdrive_test.py
--rw-r--r--   0        0        0    22036 2024-04-15 18:11:44.244159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_chain.py
--rw-r--r--   0        0        0    55070 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive.py
--rw-r--r--   0        0        0     2233 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_agent.py
--rw-r--r--   0        0        0    37120 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_test.py
--rw-r--r--   0        0        0      127 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/__init__.py
--rw-r--r--   0        0        0     3351 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/deterministic.py
--rw-r--r--   0        0        0     3566 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/hyperdrive_policy.py
--rw-r--r--   0        0        0    22939 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/lpandarb.py
--rw-r--r--   0        0        0    14825 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/lpandarb_test.py
--rw-r--r--   0        0        0     1107 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/model_zoo_test.py
--rw-r--r--   0        0        0    21510 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/random.py
--rw-r--r--   0        0        0    13289 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/random_hold.py
--rw-r--r--   0        0        0     2795 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/random_hold_test.py
--rw-r--r--   0        0        0     3888 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/random_test.py
--rw-r--r--   0        0        0     7668 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/simple_lp.py
--rw-r--r--   0        0        0     4333 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/simple_lp_test.py
--rw-r--r--   0        0        0     5860 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/smart_long.py
--rw-r--r--   0        0        0     1788 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/policies/zoo.py
--rw-r--r--   0        0        0        0 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/__init__.py
--rw-r--r--   0        0        0     9324 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/predict.py
--rw-r--r--   0        0        0    19878 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/predict_trade_test.py
--rw-r--r--   0        0        0      463 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/__init__.py
--rw-r--r--   0        0        0     3592 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/create_and_fund_user_account.py
--rw-r--r--   0        0        0    15349 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/execute_multi_agent_trades.py
--rw-r--r--   0        0        0     9298 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/fund_agents.py
--rw-r--r--   0        0        0     5760 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/get_agent_accounts.py
--rw-r--r--   0        0        0    11746 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/run_agents.py
--rw-r--r--   0        0        0     8783 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/setup_experiment.py
--rw-r--r--   0        0        0     7145 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/trade_loop.py
--rw-r--r--   0        0        0      290 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/__init__.py
--rw-r--r--   0        0        0    16400 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_long_short_maturity_values.py
--rw-r--r--   0        0        0    19256 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_path_independence.py
--rw-r--r--   0        0        0    16123 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_present_value.py
--rw-r--r--   0        0        0    13732 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_profit_check.py
--rw-r--r--   0        0        0      363 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/__init__.py
--rw-r--r--   0        0        0     2963 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/advance_time.py
--rw-r--r--   0        0        0     2028 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/close_random_trades.py
--rw-r--r--   0        0        0     7061 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/execute_random_trades.py
--rw-r--r--   0        0        0      681 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/fuzz_assertion_exception.py
--rw-r--r--   0        0        0     4881 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/setup_fuzz.py
--rw-r--r--   0        0        0     4460 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/interactive_fuzz/run_all_fuzz_tests.py
--rw-r--r--   0        0        0       58 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/test_fixtures/__init__.py
--rw-r--r--   0        0        0     1587 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/test_fixtures/chain.py
--rw-r--r--   0        0        0      141 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/test_utils/__init__.py
--rw-r--r--   0        0        0      462 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/test_utils/assert_never.py
--rw-r--r--   0        0        0     4201 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/core/test_utils/cycle_trade_policy.py
--rw-r--r--   0        0        0       72 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/__init__.py
--rw-r--r--   0        0        0      707 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/__init__.py
--rw-r--r--   0        0        0       91 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/abi/__init__.py
--rw-r--r--   0        0        0     2864 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/abi/load_abis.py
--rw-r--r--   0        0        0       86 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/contract/__init__.py
--rw-r--r--   0        0        0     1722 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/contract/deploy_contract.py
--rw-r--r--   0        0        0      201 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/errors/__init__.py
--rw-r--r--   0        0        0     3086 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/errors/errors.py
--rw-r--r--   0        0        0     1877 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/errors/errors_test.py
--rw-r--r--   0        0        0      427 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/errors/types.py
--rw-r--r--   0        0        0     3471 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/receipts.py
--rw-r--r--   0        0        0     2236 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/retry_utils.py
--rw-r--r--   0        0        0     1556 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/retry_utils_test.py
--rw-r--r--   0        0        0     1831 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/rpc_interface.py
--rw-r--r--   0        0        0    43329 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/transactions.py
--rw-r--r--   0        0        0     1746 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/base/web3_setup.py
--rw-r--r--   0        0        0     2492 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/eth_config.py
--rw-r--r--   0        0        0     4922 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/eth_config_test.py
--rw-r--r--   0        0        0      618 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/__init__.py
--rw-r--r--   0        0        0     1998 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/addresses.py
--rw-r--r--   0        0        0     2041 2024-04-15 18:11:44.248159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/assets.py
--rw-r--r--   0        0        0    18331 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/deploy.py
--rw-r--r--   0        0        0      170 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/__init__.py
--rw-r--r--   0        0        0     1309 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/_block_getters.py
--rw-r--r--   0        0        0    24789 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/_contract_calls.py
--rw-r--r--   0        0        0    11295 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/_mock_contract.py
--rw-r--r--   0        0        0     1903 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/interface_test.py
--rw-r--r--   0        0        0    42374 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_interface.py
--rw-r--r--   0        0        0    10904 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_interface_test.py
--rw-r--r--   0        0        0    15545 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_write_interface.py
--rw-r--r--   0        0        0     1546 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_write_interface_test.py
--rw-r--r--   0        0        0     2032 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/receipt_breakdown.py
--rw-r--r--   0        0        0       99 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/state/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/state/pool_state.py
--rw-r--r--   0        0        0     9626 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/hyperdrive/transactions.py
--rw-r--r--   0        0        0      251 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/test_fixtures/__init__.py
--rw-r--r--   0        0        0     9028 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/test_fixtures/deployed_pool.py
--rw-r--r--   0        0        0     3260 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/test_fixtures/interface.py
--rw-r--r--   0        0        0     1349 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/ethpy/test_fixtures/local_chain.py
--rw-r--r--   0        0        0       38 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hyperlogs/README.md
--rw-r--r--   0        0        0      467 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hyperlogs/__init__.py
--rw-r--r--   0        0        0     2338 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hyperlogs/json_encoder.py
--rw-r--r--   0        0        0    11074 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hyperlogs/logs.py
--rw-r--r--   0        0        0     3444 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hyperlogs/logs_test.py
--rw-r--r--   0        0        0     2979 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hyperlogs/rollbar_utilities.py
--rw-r--r--   0        0        0     1733 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/README.md
--rw-r--r--   0        0        0       92 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/fixedpoint_types.py
--rw-r--r--   0        0        0    26066 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC20ForwarderFactoryContract.py
--rw-r--r--   0        0        0   106156 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC20MintableContract.py
--rw-r--r--   0        0        0     3539 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC20MintableTypes.py
--rw-r--r--   0        0        0    26347 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC4626HyperdriveCoreDeployerContract.py
--rw-r--r--   0        0        0   112779 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC4626HyperdriveDeployerCoordinatorContract.py
--rw-r--r--   0        0        0    46669 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target0DeployerContract.py
--rw-r--r--   0        0        0    50531 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target1DeployerContract.py
--rw-r--r--   0        0        0    49969 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target2DeployerContract.py
--rw-r--r--   0        0        0    51725 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target3DeployerContract.py
--rw-r--r--   0        0        0    51729 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target4DeployerContract.py
--rw-r--r--   0        0        0     1386 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/HyperdriveDeployerCoordinatorTypes.py
--rw-r--r--   0        0        0   270770 2024-04-15 18:11:44.252159 agent0-0.18.0/src/agent0/hypertypes/types/HyperdriveFactoryContract.py
--rw-r--r--   0        0        0    10954 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/types/HyperdriveFactoryTypes.py
--rw-r--r--   0        0        0   251847 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/types/IHyperdriveContract.py
--rw-r--r--   0        0        0    17223 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/types/IHyperdriveTypes.py
--rw-r--r--   0        0        0   148131 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/types/MockERC4626Contract.py
--rw-r--r--   0        0        0     4368 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/types/MockERC4626Types.py
--rw-r--r--   0        0        0     1066 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/types/__init__.py
--rw-r--r--   0        0        0     4524 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/types/utilities.py
--rw-r--r--   0        0        0        0 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/utilities/__init__.py
--rw-r--r--   0        0        0     8804 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/hypertypes/utilities/conversions.py
--rw-r--r--   0        0        0      669 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/traiderdaive/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/traiderdaive/gym_environments/__init__.py
--rw-r--r--   0        0        0    23647 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/traiderdaive/gym_environments/full_hyperdrive_env.py
--rw-r--r--   0        0        0    16954 2024-04-15 18:11:44.256159 agent0-0.18.0/src/agent0/traiderdaive/gym_environments/simple_hyperdrive_env.py
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 agent0-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0     4888 2024-04-17 00:47:53.111709 agent0-0.18.1/README.md
+-rw-r--r--   0        0        0     4247 2024-04-17 00:47:53.127709 agent0-0.18.1/pyproject.toml
+-rw-r--r--   0        0        0      463 2024-04-17 00:47:53.127709 agent0-0.18.1/src/agent0/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-17 00:47:53.127709 agent0-0.18.1/src/agent0/chainsync/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-17 00:47:53.127709 agent0-0.18.1/src/agent0/chainsync/analysis/__init__.py
+-rw-r--r--   0        0        0      876 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/analysis/calc_base_buffer.py
+-rw-r--r--   0        0        0     1130 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/analysis/calc_fixed_rate.py
+-rw-r--r--   0        0        0     5570 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/analysis/calc_pnl.py
+-rw-r--r--   0        0        0     1564 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/analysis/calc_spot_price.py
+-rw-r--r--   0        0        0     2140 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/analysis/calc_ticker.py
+-rw-r--r--   0        0        0    10619 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/analysis/data_to_analysis.py
+-rw-r--r--   0        0        0      581 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/__init__.py
+-rw-r--r--   0        0        0      620 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/build_fixed_rate.py
+-rw-r--r--   0        0        0     1608 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/build_leaderboard.py
+-rw-r--r--   0        0        0     1268 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/build_ohlcv.py
+-rw-r--r--   0        0        0      546 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/build_outstanding_positions.py
+-rw-r--r--   0        0        0     1250 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/build_ticker.py
+-rw-r--r--   0        0        0      720 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/build_variable_rate.py
+-rw-r--r--   0        0        0     1038 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/plot_fixed_rate.py
+-rw-r--r--   0        0        0      858 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/plot_ohlcv.py
+-rw-r--r--   0        0        0      851 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/plot_outstanding_positions.py
+-rw-r--r--   0        0        0     1117 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/plot_utils.py
+-rw-r--r--   0        0        0     4630 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/dashboard/usernames.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/api/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/api/api_interface.py
+-rw-r--r--   0        0        0     4334 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/api/api_server.py
+-rw-r--r--   0        0        0      388 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/base/__init__.py
+-rw-r--r--   0        0        0    12480 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/base/interface.py
+-rw-r--r--   0        0        0    10937 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/base/interface_test.py
+-rw-r--r--   0        0        0     1648 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/base/schema.py
+-rw-r--r--   0        0        0     2742 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/base/schema_test.py
+-rw-r--r--   0        0        0     1084 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/__init__.py
+-rw-r--r--   0        0        0     4303 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/chain_to_db.py
+-rw-r--r--   0        0        0    21417 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/convert_data.py
+-rw-r--r--   0        0        0     8207 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/import_export_data.py
+-rw-r--r--   0        0        0     1218 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/import_export_data_test.py
+-rw-r--r--   0        0        0    30568 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/interface.py
+-rw-r--r--   0        0        0    21353 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/interface_test.py
+-rw-r--r--   0        0        0    15387 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/schema.py
+-rw-r--r--   0        0        0     8085 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/schema_test.py
+-rw-r--r--   0        0        0      121 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/exec/__init__.py
+-rw-r--r--   0        0        0     5884 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/exec/acquire_data.py
+-rw-r--r--   0        0        0     6210 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/exec/data_analysis.py
+-rw-r--r--   0        0        0     1919 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/postgres_config.py
+-rw-r--r--   0        0        0     4066 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/streamlit/Dashboard.py
+-rw-r--r--   0        0        0     7174 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/streamlit/pages/Wallet_Stats.py
+-rw-r--r--   0        0        0      149 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/test_fixtures/__init__.py
+-rw-r--r--   0        0        0     6763 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/test_fixtures/db_session.py
+-rw-r--r--   0        0        0     1265 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/chainsync/test_fixtures/dummy_session.py
+-rw-r--r--   0        0        0      218 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/__init__.py
+-rw-r--r--   0        0        0     8781 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/accounts_config.py
+-rw-r--r--   0        0        0      215 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/agent/__init__.py
+-rw-r--r--   0        0        0     3881 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/agent/eth_agent.py
+-rw-r--r--   0        0        0     4839 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/agent/eth_wallet.py
+-rw-r--r--   0        0        0      954 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/agent/eth_wallet_test.py
+-rw-r--r--   0        0        0      414 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/agent/market_actions.py
+-rw-r--r--   0        0        0      174 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/config/__init__.py
+-rw-r--r--   0        0        0     1237 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/config/agent_config.py
+-rw-r--r--   0        0        0     1513 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/config/budget.py
+-rw-r--r--   0        0        0     4628 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/config/environment_config.py
+-rw-r--r--   0        0        0      747 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/make_key.py
+-rw-r--r--   0        0        0      152 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/policies/__init__.py
+-rw-r--r--   0        0        0     3407 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/policies/base.py
+-rw-r--r--   0        0        0     1368 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/policies/no_action.py
+-rw-r--r--   0        0        0     6101 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/types.py
+-rw-r--r--   0        0        0     7199 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/base/types_test.py
+-rw-r--r--   0        0        0      290 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/__init__.py
+-rw-r--r--   0        0        0      606 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/agent/__init__.py
+-rw-r--r--   0        0        0     8046 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/agent/build_wallet_positions.py
+-rw-r--r--   0        0        0    10266 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_actions.py
+-rw-r--r--   0        0        0     5425 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_agent.py
+-rw-r--r--   0        0        0     7871 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_wallet.py
+-rw-r--r--   0        0        0     2300 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_wallet_test.py
+-rw-r--r--   0        0        0     2976 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/agent/trade_result.py
+-rw-r--r--   0        0        0      326 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/crash_report/__init__.py
+-rw-r--r--   0        0        0    17230 2024-04-17 00:47:53.131709 agent0-0.18.1/src/agent0/core/hyperdrive/crash_report/crash_report.py
+-rw-r--r--   0        0        0     9953 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/crash_report/known_error_checks.py
+-rw-r--r--   0        0        0      184 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/econ_tests.py
+-rw-r--r--   0        0        0     6061 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/event_types.py
+-rw-r--r--   0        0        0      241 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/exec/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/exec/check_for_new_block.py
+-rw-r--r--   0        0        0    17377 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/exec/execute_agent_trades.py
+-rw-r--r--   0        0        0     1284 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/exec/set_max_approval.py
+-rw-r--r--   0        0        0     1346 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_chain.py
+-rw-r--r--   0        0        0    23041 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_hyperdrive.py
+-rw-r--r--   0        0        0     8207 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_hyperdrive_agent.py
+-rw-r--r--   0        0        0    16478 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_hyperdrive_test.py
+-rw-r--r--   0        0        0    22036 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_chain.py
+-rw-r--r--   0        0        0    55070 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive.py
+-rw-r--r--   0        0        0     2233 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_agent.py
+-rw-r--r--   0        0        0    37120 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_test.py
+-rw-r--r--   0        0        0      127 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/__init__.py
+-rw-r--r--   0        0        0     3351 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/deterministic.py
+-rw-r--r--   0        0        0     3566 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/hyperdrive_policy.py
+-rw-r--r--   0        0        0    23297 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/lpandarb.py
+-rw-r--r--   0        0        0    14825 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/lpandarb_test.py
+-rw-r--r--   0        0        0     1107 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/model_zoo_test.py
+-rw-r--r--   0        0        0    21510 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/random.py
+-rw-r--r--   0        0        0    13321 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/random_hold.py
+-rw-r--r--   0        0        0     2795 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/random_hold_test.py
+-rw-r--r--   0        0        0     3888 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/random_test.py
+-rw-r--r--   0        0        0     7668 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/simple_lp.py
+-rw-r--r--   0        0        0     4333 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/simple_lp_test.py
+-rw-r--r--   0        0        0     5860 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/smart_long.py
+-rw-r--r--   0        0        0     1788 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/policies/zoo.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/__init__.py
+-rw-r--r--   0        0        0     9324 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/predict.py
+-rw-r--r--   0        0        0    19878 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/predict_trade_test.py
+-rw-r--r--   0        0        0      463 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/__init__.py
+-rw-r--r--   0        0        0     3592 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/create_and_fund_user_account.py
+-rw-r--r--   0        0        0    15360 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/execute_multi_agent_trades.py
+-rw-r--r--   0        0        0     9298 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/fund_agents.py
+-rw-r--r--   0        0        0     5760 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/get_agent_accounts.py
+-rw-r--r--   0        0        0    11746 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/run_agents.py
+-rw-r--r--   0        0        0     8783 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/setup_experiment.py
+-rw-r--r--   0        0        0     7145 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/trade_loop.py
+-rw-r--r--   0        0        0      290 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/__init__.py
+-rw-r--r--   0        0        0    16400 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_long_short_maturity_values.py
+-rw-r--r--   0        0        0    19256 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_path_independence.py
+-rw-r--r--   0        0        0    16123 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_present_value.py
+-rw-r--r--   0        0        0    13732 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_profit_check.py
+-rw-r--r--   0        0        0      363 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/__init__.py
+-rw-r--r--   0        0        0     2963 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/advance_time.py
+-rw-r--r--   0        0        0     2028 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/close_random_trades.py
+-rw-r--r--   0        0        0     7061 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/execute_random_trades.py
+-rw-r--r--   0        0        0      681 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/fuzz_assertion_exception.py
+-rw-r--r--   0        0        0     4881 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/setup_fuzz.py
+-rw-r--r--   0        0        0     4460 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/interactive_fuzz/run_all_fuzz_tests.py
+-rw-r--r--   0        0        0       58 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/test_fixtures/__init__.py
+-rw-r--r--   0        0        0     1587 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/test_fixtures/chain.py
+-rw-r--r--   0        0        0      141 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/test_utils/__init__.py
+-rw-r--r--   0        0        0      462 2024-04-17 00:47:53.135710 agent0-0.18.1/src/agent0/core/test_utils/assert_never.py
+-rw-r--r--   0        0        0     4201 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/core/test_utils/cycle_trade_policy.py
+-rw-r--r--   0        0        0       72 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/abi/__init__.py
+-rw-r--r--   0        0        0     2864 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/abi/load_abis.py
+-rw-r--r--   0        0        0       86 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/contract/__init__.py
+-rw-r--r--   0        0        0     1722 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/contract/deploy_contract.py
+-rw-r--r--   0        0        0      201 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/errors/__init__.py
+-rw-r--r--   0        0        0     3086 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/errors/errors.py
+-rw-r--r--   0        0        0     1877 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/errors/errors_test.py
+-rw-r--r--   0        0        0      427 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/errors/types.py
+-rw-r--r--   0        0        0     3471 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/receipts.py
+-rw-r--r--   0        0        0     2236 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/retry_utils.py
+-rw-r--r--   0        0        0     1556 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/retry_utils_test.py
+-rw-r--r--   0        0        0     1831 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/rpc_interface.py
+-rw-r--r--   0        0        0    43329 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/transactions.py
+-rw-r--r--   0        0        0     1746 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/base/web3_setup.py
+-rw-r--r--   0        0        0     2492 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/eth_config.py
+-rw-r--r--   0        0        0     4922 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/eth_config_test.py
+-rw-r--r--   0        0        0      618 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/__init__.py
+-rw-r--r--   0        0        0     1998 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/addresses.py
+-rw-r--r--   0        0        0     2041 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/assets.py
+-rw-r--r--   0        0        0    18331 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/deploy.py
+-rw-r--r--   0        0        0      170 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/__init__.py
+-rw-r--r--   0        0        0     1309 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/_block_getters.py
+-rw-r--r--   0        0        0    24789 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/_contract_calls.py
+-rw-r--r--   0        0        0    11295 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/_mock_contract.py
+-rw-r--r--   0        0        0     1903 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/interface_test.py
+-rw-r--r--   0        0        0    42374 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_interface.py
+-rw-r--r--   0        0        0    10904 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_interface_test.py
+-rw-r--r--   0        0        0    15545 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_write_interface.py
+-rw-r--r--   0        0        0     1546 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_write_interface_test.py
+-rw-r--r--   0        0        0     2032 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/receipt_breakdown.py
+-rw-r--r--   0        0        0       99 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/state/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/state/pool_state.py
+-rw-r--r--   0        0        0     9626 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/hyperdrive/transactions.py
+-rw-r--r--   0        0        0      251 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/test_fixtures/__init__.py
+-rw-r--r--   0        0        0     9028 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/test_fixtures/deployed_pool.py
+-rw-r--r--   0        0        0     3260 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/test_fixtures/interface.py
+-rw-r--r--   0        0        0     1349 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/ethpy/test_fixtures/local_chain.py
+-rw-r--r--   0        0        0       38 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hyperlogs/README.md
+-rw-r--r--   0        0        0      467 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hyperlogs/__init__.py
+-rw-r--r--   0        0        0     2338 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hyperlogs/json_encoder.py
+-rw-r--r--   0        0        0    11074 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hyperlogs/logs.py
+-rw-r--r--   0        0        0     3444 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hyperlogs/logs_test.py
+-rw-r--r--   0        0        0     2979 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hyperlogs/rollbar_utilities.py
+-rw-r--r--   0        0        0     1733 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hypertypes/README.md
+-rw-r--r--   0        0        0       92 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hypertypes/__init__.py
+-rw-r--r--   0        0        0     2316 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hypertypes/fixedpoint_types.py
+-rw-r--r--   0        0        0    26066 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hypertypes/types/ERC20ForwarderFactoryContract.py
+-rw-r--r--   0        0        0   106156 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hypertypes/types/ERC20MintableContract.py
+-rw-r--r--   0        0        0     3539 2024-04-17 00:47:53.139710 agent0-0.18.1/src/agent0/hypertypes/types/ERC20MintableTypes.py
+-rw-r--r--   0        0        0    26347 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/ERC4626HyperdriveCoreDeployerContract.py
+-rw-r--r--   0        0        0   112779 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/ERC4626HyperdriveDeployerCoordinatorContract.py
+-rw-r--r--   0        0        0    46669 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target0DeployerContract.py
+-rw-r--r--   0        0        0    50531 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target1DeployerContract.py
+-rw-r--r--   0        0        0    49969 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target2DeployerContract.py
+-rw-r--r--   0        0        0    51725 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target3DeployerContract.py
+-rw-r--r--   0        0        0    51729 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target4DeployerContract.py
+-rw-r--r--   0        0        0     1386 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/HyperdriveDeployerCoordinatorTypes.py
+-rw-r--r--   0        0        0   270770 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/HyperdriveFactoryContract.py
+-rw-r--r--   0        0        0    10954 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/HyperdriveFactoryTypes.py
+-rw-r--r--   0        0        0   251847 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/IHyperdriveContract.py
+-rw-r--r--   0        0        0    17223 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/IHyperdriveTypes.py
+-rw-r--r--   0        0        0   148131 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/MockERC4626Contract.py
+-rw-r--r--   0        0        0     4368 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/MockERC4626Types.py
+-rw-r--r--   0        0        0     1066 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/__init__.py
+-rw-r--r--   0        0        0     4524 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/types/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/utilities/__init__.py
+-rw-r--r--   0        0        0     8804 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/hypertypes/utilities/conversions.py
+-rw-r--r--   0        0        0      669 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/traiderdaive/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/traiderdaive/gym_environments/__init__.py
+-rw-r--r--   0        0        0    23647 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/traiderdaive/gym_environments/full_hyperdrive_env.py
+-rw-r--r--   0        0        0    16954 2024-04-17 00:47:53.143710 agent0-0.18.1/src/agent0/traiderdaive/gym_environments/simple_hyperdrive_env.py
+-rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 agent0-0.18.1/PKG-INFO
```

### Comparing `agent0-0.18.0/README.md` & `agent0-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/pyproject.toml` & `agent0-0.18.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "agent0"
-version = "0.18.0"
+version = "0.18.1"
 # Authors are the current, primary stuards of the repo
 # contributors can be found on github
 authors = [
     { name = "Dylan Paiton", email = "dylan@delv.tech" },
     { name = "Mihai Cosma", email = "mihai@delv.tech" },
     { name = "Matthew Brown", email = "matt@delv.tech" },
     { name = "Sheng Lundquist", email = "sheng@delv.tech" },
@@ -23,19 +23,20 @@
     "Development Status :: 3 - Alpha",
     "Natural Language :: English",
 ]
 
 dependencies = [
     "dill",
     "docker",
+    "eth-typing==4.1.0",
     "fixedpointmath",
     "flask",
     "flask-expects-json",
     "hexbytes",
-    "hyperdrivepy==0.13.0",
+    "hyperdrivepy==1.0.1",
     "ipython",
     "matplotlib",
     "mplfinance",
     "nest_asyncio",
     "numpy",
     "pandas",
     "pandas-stubs",
```

### Comparing `agent0-0.18.0/src/agent0/chainsync/analysis/calc_base_buffer.py` & `agent0-0.18.1/src/agent0/chainsync/analysis/calc_base_buffer.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/analysis/calc_fixed_rate.py` & `agent0-0.18.1/src/agent0/chainsync/analysis/calc_fixed_rate.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/analysis/calc_pnl.py` & `agent0-0.18.1/src/agent0/chainsync/analysis/calc_pnl.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/analysis/calc_spot_price.py` & `agent0-0.18.1/src/agent0/chainsync/analysis/calc_spot_price.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/analysis/calc_ticker.py` & `agent0-0.18.1/src/agent0/chainsync/analysis/calc_ticker.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/analysis/data_to_analysis.py` & `agent0-0.18.1/src/agent0/chainsync/analysis/data_to_analysis.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/__init__.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/build_fixed_rate.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/build_fixed_rate.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/build_leaderboard.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/build_leaderboard.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/build_ohlcv.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/build_ohlcv.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/build_outstanding_positions.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/build_outstanding_positions.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/build_ticker.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/build_ticker.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/build_variable_rate.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/build_variable_rate.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/plot_fixed_rate.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/plot_fixed_rate.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/plot_ohlcv.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/plot_ohlcv.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/plot_outstanding_positions.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/plot_outstanding_positions.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/plot_utils.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/plot_utils.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/dashboard/usernames.py` & `agent0-0.18.1/src/agent0/chainsync/dashboard/usernames.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/api/api_interface.py` & `agent0-0.18.1/src/agent0/chainsync/db/api/api_interface.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/api/api_server.py` & `agent0-0.18.1/src/agent0/chainsync/db/api/api_server.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/base/interface.py` & `agent0-0.18.1/src/agent0/chainsync/db/base/interface.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/base/interface_test.py` & `agent0-0.18.1/src/agent0/chainsync/db/base/interface_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/base/schema.py` & `agent0-0.18.1/src/agent0/chainsync/db/base/schema.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/base/schema_test.py` & `agent0-0.18.1/src/agent0/chainsync/db/base/schema_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/__init__.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/__init__.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/chain_to_db.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/chain_to_db.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/convert_data.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/convert_data.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/import_export_data.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/import_export_data.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/import_export_data_test.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/import_export_data_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/interface.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/interface.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/interface_test.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/interface_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/schema.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/schema.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/db/hyperdrive/schema_test.py` & `agent0-0.18.1/src/agent0/chainsync/db/hyperdrive/schema_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/exec/acquire_data.py` & `agent0-0.18.1/src/agent0/chainsync/exec/acquire_data.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/exec/data_analysis.py` & `agent0-0.18.1/src/agent0/chainsync/exec/data_analysis.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/postgres_config.py` & `agent0-0.18.1/src/agent0/chainsync/postgres_config.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/streamlit/Dashboard.py` & `agent0-0.18.1/src/agent0/chainsync/streamlit/Dashboard.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/streamlit/pages/Wallet_Stats.py` & `agent0-0.18.1/src/agent0/chainsync/streamlit/pages/Wallet_Stats.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/test_fixtures/db_session.py` & `agent0-0.18.1/src/agent0/chainsync/test_fixtures/db_session.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/chainsync/test_fixtures/dummy_session.py` & `agent0-0.18.1/src/agent0/chainsync/test_fixtures/dummy_session.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/accounts_config.py` & `agent0-0.18.1/src/agent0/core/accounts_config.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/agent/eth_agent.py` & `agent0-0.18.1/src/agent0/core/base/agent/eth_agent.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/agent/eth_wallet.py` & `agent0-0.18.1/src/agent0/core/base/agent/eth_wallet.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/agent/eth_wallet_test.py` & `agent0-0.18.1/src/agent0/core/base/agent/eth_wallet_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/config/agent_config.py` & `agent0-0.18.1/src/agent0/core/base/config/agent_config.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/config/budget.py` & `agent0-0.18.1/src/agent0/core/base/config/budget.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/config/environment_config.py` & `agent0-0.18.1/src/agent0/core/base/config/environment_config.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/make_key.py` & `agent0-0.18.1/src/agent0/core/base/make_key.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/policies/base.py` & `agent0-0.18.1/src/agent0/core/base/policies/base.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/policies/no_action.py` & `agent0-0.18.1/src/agent0/core/base/policies/no_action.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/types.py` & `agent0-0.18.1/src/agent0/core/base/types.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/base/types_test.py` & `agent0-0.18.1/src/agent0/core/base/types_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/agent/__init__.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/agent/build_wallet_positions.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/agent/build_wallet_positions.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_actions.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_actions.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_agent.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_agent.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_wallet.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_wallet.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/agent/hyperdrive_wallet_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/agent/hyperdrive_wallet_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/agent/trade_result.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/agent/trade_result.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/crash_report/crash_report.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/crash_report/crash_report.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/crash_report/known_error_checks.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/crash_report/known_error_checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Helper functions for checking for known errors in contract calls."""
 
-from web3.exceptions import ContractCustomError, ContractLogicError
+from web3.exceptions import ContractCustomError
 
 from agent0.core.hyperdrive import HyperdriveActionType, TradeResult
 from agent0.core.test_utils import assert_never
 from agent0.ethpy.base.errors import ContractCallException
+from agent0.ethpy.hyperdrive import HyperdriveReadInterface
 
 
-def check_for_invalid_balance(trade_result: TradeResult) -> TradeResult:
+# pylint: disable=too-many-statements
+def check_for_invalid_balance(trade_result: TradeResult, interface: HyperdriveReadInterface) -> TradeResult:
     """Detects invalid balance errors in trade_result and adds additional information to the
-    exception in trade_result
+    exception in trade_result.
 
     Arguments
     ---------
     trade_result: TradeResult
-        The trade result object from trading
+        The trade result object from trading.
+    interface: HyperdriveReadInterface
+        The hyperdrive read interface to compute expected balances for trades.
 
     Returns
     -------
     TradeResult
         A modified trade_result that has a custom exception argument message prepended
     """
     assert trade_result.agent is not None
@@ -55,30 +59,32 @@
                     invalid_balance = True
                     add_arg = (
                         f"Invalid balance: {trade_type.name} for {trade_amount} long-{maturity_time}, "
                         f"balance of {wallet.longs[maturity_time].balance} long-{maturity_time}."
                     )
 
         case HyperdriveActionType.OPEN_SHORT:
-            # We can't check for invalid balance here since the trade_amount is in units of bonds, and the
-            # amount of base needed for the short isn't available. However, the exception itself has the
-            # "ERC20: transfer amount exceeds balance" error, so should be okay.
-            # TODO this should be solvable using some sort of preview, but the above error might be sufficient.
-
-            # We explicitly check for the error here to set flag
-            # TODO this catch is not guaranteed to be correct in the future.
-            if (
-                isinstance(trade_result.exception, ContractCallException)
-                and isinstance(trade_result.exception.orig_exception, ContractLogicError)
-                and ("ERC20: transfer amount exceeds balance" in trade_result.exception.args[0])
-            ):
+            # We use the interface to calculate the amount of deposit required to open
+            # the provided short.
+            # TODO there may be a race condition here if the block ticks while handling this crash
+
+            # We catch all errors thrown by calc open short in rust. If the underlying function
+            # fails, it's likely not an invalid balance issue.
+            base_deposit = None
+            try:
+                base_deposit = interface.calc_open_short(trade_amount)
+            except BaseException:  # pylint: disable=broad-except
+                pass
+
+            if base_deposit is not None and base_deposit > wallet.balance.amount:
                 invalid_balance = True
                 add_arg = (
-                    f"Invalid balance: {trade_type.name} for {trade_amount} bonds, ",
-                    f"balance of {wallet.balance.amount} {wallet.balance.unit.name}.",
+                    f"Invalid balance: {trade_type.name} for {trade_amount} bonds, "
+                    f"expected deposit of {base_deposit} {wallet.balance.unit.name}, "
+                    f"balance of {wallet.balance.amount} {wallet.balance.unit.name}."
                 )
 
         case HyperdriveActionType.CLOSE_SHORT:
             # Short doesn't exist
             if maturity_time not in wallet.shorts:
                 invalid_balance = True
                 add_arg = (
```

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/econ_tests.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/econ_tests.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/event_types.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/event_types.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/exec/check_for_new_block.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/exec/check_for_new_block.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/exec/execute_agent_trades.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/exec/execute_agent_trades.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,17 @@
                 for i, trade_object in enumerate(trades)
             ],
             # Instead of throwing exception, return the exception to the caller here
             return_exceptions=True,
         )
     )
 
-    trade_results, wallet_updates = _handle_contract_call_to_trade(wallet_deltas_or_exception, trades, interface, agent)
-
-    # The wallet update after should be fine, since we can see what trades went through
-    # and only apply those wallet deltas. Wallet deltas are also invariant to order
-    # as long as the transaction went through.
-    for wallet_delta in wallet_updates:
-        agent.wallet.update(wallet_delta)
+    trade_results = _handle_contract_call_to_trade_and_update_wallets(
+        wallet_deltas_or_exception, trades, interface, agent
+    )
 
     # TODO to avoid adding a post action in base policy, we only call post action
     # if the policy is a hyperdrive policy. Ideally, we'd allow base classes all the
     # way down
     if isinstance(agent.policy, HyperdriveBasePolicy):
         # Calls the agent with the trade results in case the policy needs to do bookkeeping.
         # We copy a trade results to avoid changing the original trade result for crash reporting.
@@ -165,24 +161,19 @@
     nonce = retry_call(DEFAULT_READ_RETRY_COUNT, None, interface.web3.eth.get_transaction_count, agent.checksum_address)
 
     try:
         wallet_delta_or_exception = await _async_match_contract_call_to_trade(agent, interface, trade_object, nonce)
     except Exception as e:  # pylint: disable=broad-except
         wallet_delta_or_exception = e
 
-    trade_results, wallet_updates = _handle_contract_call_to_trade(
+    trade_results = _handle_contract_call_to_trade_and_update_wallets(
         [wallet_delta_or_exception], [trade_object], interface, agent
     )
 
     assert len(trade_results) == 1
-    # Wallet updates will be 0 if the trade failed
-    assert len(wallet_updates) <= 1
-
-    for wallet_delta in wallet_updates:
-        agent.wallet.update(wallet_delta)
 
     # Some policies still need to bookkeep if single trades are being made. We call that here.
     # TODO to avoid adding a post action in base policy, we only call post action
     # if the policy is a hyperdrive policy. Ideally, we'd allow base classes all the
     # way down
     if execute_policy_post_action and isinstance(agent.policy, HyperdriveBasePolicy):
         # Calls the agent with the trade results in case the policy needs to do bookkeeping.
@@ -193,21 +184,21 @@
         #
         # TODO can't put post_action in agent due to circular import, so we call the policy post_action here
         agent.policy.post_action(interface, deepcopy(trade_results))
 
     return trade_results[0]
 
 
-def _handle_contract_call_to_trade(
+def _handle_contract_call_to_trade_and_update_wallets(
     wallet_deltas_or_exception: list[tuple[HyperdriveWalletDeltas, ReceiptBreakdown] | BaseException],
     trades: list[Trade[HyperdriveMarketAction]],
     interface: HyperdriveReadInterface,
     agent: HyperdriveAgent,
-):
-    """Handle the results of executing trades.
+) -> list[TradeResult]:
+    """Handle the results of executing trades. This function also updates the underlying agent's wallet.
 
     Arguments
     ---------
     wallet_deltas_or_exception: list[tuple[HyperdriveWalletDeltas, ReceiptBreakdown] | BaseException]
         The results of executing trades. This argument is either the output of
         _async_match_contract_call_to_trade or an exception to crash report.
     trades: list[HyperdriveMarketAction]
@@ -215,52 +206,56 @@
     interface: HyperdriveReadInterface
         The read interface for the market.
     agent: HyperdriveAgent
         The agent that executed the trades.
 
     Returns
     -------
-    Tuple[list[TradeResult], list[HyperdriveWalletDeltas]]
-        Returns the list of trade results, as well as any wallet deltas that need to be
-        applied to the agent.
+    list[TradeResult]
+        Returns the list of trade results.
     """
 
     # Sanity check
     if len(wallet_deltas_or_exception) != len(trades):
         raise AssertionError(
             "The number of wallet deltas should match the number of trades, but does not."
             f"\n{wallet_deltas_or_exception=}\n{trades=}"
         )
 
     trade_results: list[TradeResult] = []
-    wallet_deltas: list[HyperdriveWalletDeltas] = []
+    # Since the list of wallet deltas or exceptions is guaranteed to be in the order
+    # of execution, we incrementally update the wallet. Updating the wallet
+    # while iterating will ensure the invalid balance check has the most
+    # up to date wallet for checking balances.
     for result, trade_object in zip(wallet_deltas_or_exception, trades):
         if isinstance(result, Exception):
             trade_result = build_crash_trade_result(result, interface, agent, trade_object)
             # We check for common errors and allow for custom handling of various errors.
             # These functions adjust the trade_result.exception object to add
             # additional arguments describing these detected errors for crash reporting.
-            trade_result = check_for_invalid_balance(trade_result)
+            trade_result = check_for_invalid_balance(trade_result, interface)
             trade_result = check_for_slippage(trade_result)
             trade_result = check_for_min_txn_amount(trade_result)
         else:
             if not isinstance(result, tuple):
                 raise TypeError("The trade result is not the correct type.")
             if not len(result) == 2:
                 raise AssertionError("The trade result is improperly formatted.")
             wallet_delta, tx_receipt = result
             if not isinstance(wallet_delta, HyperdriveWalletDeltas) or not isinstance(tx_receipt, ReceiptBreakdown):
                 raise TypeError("The wallet deltas or the transaction receipt is not the correct type.")
-            wallet_deltas.append(wallet_delta)
+
+            agent.wallet.update(wallet_delta)
+
             trade_result = TradeResult(
                 status=TradeStatus.SUCCESS, agent=agent, trade_object=trade_object, tx_receipt=tx_receipt
             )
         trade_results.append(trade_result)
 
-    return trade_results, wallet_deltas
+    return trade_results
 
 
 async def _async_match_contract_call_to_trade(
     agent: HyperdriveAgent,
     interface: HyperdriveReadWriteInterface,
     trade_envelope: Trade[HyperdriveMarketAction],
     nonce: Nonce,
```

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/exec/set_max_approval.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/exec/set_max_approval.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_chain.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_chain.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_hyperdrive.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_hyperdrive.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_hyperdrive_agent.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_hyperdrive_agent.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_hyperdrive_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_hyperdrive_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_chain.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_chain.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_agent.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_agent.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/interactive/i_local_hyperdrive_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/deterministic.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/deterministic.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/hyperdrive_policy.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/hyperdrive_policy.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/lpandarb.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/lpandarb.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,28 +89,28 @@
         curve_portion = maximum(
             FixedPoint(0),
             FixedPoint((maturity_time - pool_state.block_time + 12))
             / FixedPoint(interface.pool_config.position_duration),
         )
         logging.info("curve portion is %s\nbonds needed is %s", curve_portion, bonds_needed)
         reduce_short_amount = minimum(
-            short.balance, bonds_needed / curve_portion, interface.calc_max_long(wallet.balance.amount, pool_state)
+            short.balance, bonds_needed / curve_portion, interface.calc_max_long(max_trade_amount_base, pool_state)
         )
         if reduce_short_amount > min_trade_amount_bonds:
             bonds_needed -= reduce_short_amount * curve_portion
             logging.debug(
                 "reducing short by %s\nreduce_short_amount*curve_portion = %s",
                 reduce_short_amount,
                 reduce_short_amount * curve_portion,
             )
             action_list.append(close_short_trade(reduce_short_amount, maturity_time, slippage_tolerance))
     # Open a new long, if there's still a need, and we have money
-    if wallet.balance.amount >= min_trade_amount_bonds and bonds_needed > min_trade_amount_bonds:
+    if max_trade_amount_base >= min_trade_amount_bonds and bonds_needed > min_trade_amount_bonds:
         max_long_shares = interface.calc_shares_in_given_bonds_out_down(
-            interface.calc_max_long(wallet.balance.amount, pool_state), pool_state
+            interface.calc_max_long(max_trade_amount_base, pool_state), pool_state
         )
         shares_needed = interface.calc_shares_in_given_bonds_out_down(bonds_needed, pool_state)
         amount_base = minimum(
             shares_needed * pool_state.pool_info.vault_share_price,
             max_long_shares * pool_state.pool_info.vault_share_price,
             max_trade_amount_base,
         )
@@ -168,23 +168,29 @@
         curve_portion = maximum(
             FixedPoint(0),
             FixedPoint(maturity_time - pool_state.block_time + 12)
             / FixedPoint(interface.pool_config.position_duration),
         )
         logging.info("curve portion is %s\nbonds needed is %s", curve_portion, bonds_needed)
         reduce_long_amount = minimum(
-            long.balance, bonds_needed / curve_portion, interface.calc_max_short(wallet.balance.amount, pool_state)
+            long.balance, bonds_needed / curve_portion, interface.calc_max_short(max_trade_amount_base, pool_state)
         )
         if reduce_long_amount > min_trade_amount_bonds:
             bonds_needed -= reduce_long_amount * curve_portion
             logging.debug("reducing long by %s", reduce_long_amount)
             action_list.append(close_long_trade(reduce_long_amount, maturity_time, slippage_tolerance))
     # Open a new short, if there's still a need, and we have money
-    if wallet.balance.amount >= min_trade_amount_bonds and bonds_needed > min_trade_amount_bonds:
-        amount_bonds = minimum(bonds_needed, interface.calc_max_short(max_trade_amount_base, pool_state))
+    if max_trade_amount_base >= min_trade_amount_bonds and bonds_needed > min_trade_amount_bonds:
+        max_short = interface.calc_max_short(max_trade_amount_base, pool_state)
+        # TODO calc_max_short seems to be a bit off wrt the budget we have, likely
+        # due to the underlying calc_open_short being off. We subtract a small amount
+        # from the max short for a fix for now to fix test.
+        # https://github.com/delvtech/hyperdrive/issues/969
+        max_short -= FixedPoint("0.1")
+        amount_bonds = minimum(bonds_needed, max_short)
         action_list.append(open_short_trade(amount_bonds, slippage_tolerance))
     return action_list
 
 
 def calc_shares_needed_for_bonds(
     interface: HyperdriveReadInterface,
     pool_state: PoolState,
```

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/lpandarb_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/lpandarb_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/model_zoo_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/model_zoo_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/random.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/random.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/random_hold.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/random_hold.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         long_to_close.txn_sent = True
 
         ignore_slippage = self.rng.choice([True, False], size=1) if self.randomly_ignore_slippage_tolerance else False
         if ignore_slippage:
             slippage = None
         else:
             slippage = self.slippage_tolerance
-        return [close_long_trade(long_to_close.bond_amount, long_to_close.maturity_time, slippage)]
+        return [close_long_trade(long_to_close.bond_amount, long_to_close.maturity_time, slippage, self.gas_limit)]
 
     def close_random_short(
         self, interface: HyperdriveReadInterface, wallet: HyperdriveWallet
     ) -> list[Trade[HyperdriveMarketAction]]:
         """Closes a random short that's ready to be closed.
 
         Arguments
@@ -228,15 +228,15 @@
         short_to_close.txn_sent = True
 
         ignore_slippage = self.rng.choice([True, False], size=1) if self.randomly_ignore_slippage_tolerance else False
         if ignore_slippage:
             slippage = None
         else:
             slippage = self.slippage_tolerance
-        return [close_short_trade(short_to_close.bond_amount, short_to_close.maturity_time, slippage)]
+        return [close_short_trade(short_to_close.bond_amount, short_to_close.maturity_time, slippage, self.gas_limit)]
 
     def post_action(self, interface: HyperdriveReadInterface, trade_results: list[TradeResult]) -> None:
         """Random hold updates open position bookkeeping based on which positions were closed.
 
         Arguments
         ---------
         interface: HyperdriveReadInterface
```

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/random_hold_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/random_hold_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/random_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/random_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/simple_lp.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/simple_lp.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/simple_lp_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/simple_lp_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/smart_long.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/smart_long.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/policies/zoo.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/policies/zoo.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/predict.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/predict.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/predict_trade_test.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/predict_trade_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/create_and_fund_user_account.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/create_and_fund_user_account.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/execute_multi_agent_trades.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/execute_multi_agent_trades.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     # Iterate through trade results, checking for known errors
     out_trade_results = []
     for trade_result in trade_results:
         if trade_result.status == TradeStatus.FAIL:
             # Here, we check for common errors and allow for custom handling of various errors
             # These functions adjust the trade_result.exception object to add
             # additional arguments describing these detected errors for crash reporting
-            trade_result = check_for_invalid_balance(trade_result)
+            trade_result = check_for_invalid_balance(trade_result, interface)
             trade_result = check_for_slippage(trade_result)
             trade_result = check_for_min_txn_amount(trade_result)
         out_trade_results.append(trade_result)
     return out_trade_results
 
 
 async def _async_execute_single_agent_trade(
```

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/fund_agents.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/fund_agents.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/get_agent_accounts.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/get_agent_accounts.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/run_agents.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/run_agents.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/setup_experiment.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/setup_experiment.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/hyperdrive/utilities/run_bots/trade_loop.py` & `agent0-0.18.1/src/agent0/core/hyperdrive/utilities/run_bots/trade_loop.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_long_short_maturity_values.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_long_short_maturity_values.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_path_independence.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_path_independence.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_present_value.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_present_value.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/fuzz_profit_check.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/fuzz_profit_check.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/advance_time.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/advance_time.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/close_random_trades.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/close_random_trades.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/execute_random_trades.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/execute_random_trades.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/fuzz_assertion_exception.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/fuzz_assertion_exception.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/helpers/setup_fuzz.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/helpers/setup_fuzz.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/interactive_fuzz/run_all_fuzz_tests.py` & `agent0-0.18.1/src/agent0/core/interactive_fuzz/run_all_fuzz_tests.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/test_fixtures/chain.py` & `agent0-0.18.1/src/agent0/core/test_fixtures/chain.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/core/test_utils/cycle_trade_policy.py` & `agent0-0.18.1/src/agent0/core/test_utils/cycle_trade_policy.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/__init__.py` & `agent0-0.18.1/src/agent0/ethpy/base/__init__.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/abi/load_abis.py` & `agent0-0.18.1/src/agent0/ethpy/base/abi/load_abis.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/contract/deploy_contract.py` & `agent0-0.18.1/src/agent0/ethpy/base/contract/deploy_contract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/errors/errors.py` & `agent0-0.18.1/src/agent0/ethpy/base/errors/errors.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/errors/errors_test.py` & `agent0-0.18.1/src/agent0/ethpy/base/errors/errors_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/receipts.py` & `agent0-0.18.1/src/agent0/ethpy/base/receipts.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/retry_utils.py` & `agent0-0.18.1/src/agent0/ethpy/base/retry_utils.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/retry_utils_test.py` & `agent0-0.18.1/src/agent0/ethpy/base/retry_utils_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/rpc_interface.py` & `agent0-0.18.1/src/agent0/ethpy/base/rpc_interface.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/transactions.py` & `agent0-0.18.1/src/agent0/ethpy/base/transactions.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/base/web3_setup.py` & `agent0-0.18.1/src/agent0/ethpy/base/web3_setup.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/eth_config.py` & `agent0-0.18.1/src/agent0/ethpy/eth_config.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/eth_config_test.py` & `agent0-0.18.1/src/agent0/ethpy/eth_config_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/__init__.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/__init__.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/addresses.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/addresses.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/assets.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/assets.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/deploy.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/deploy.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/_block_getters.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/_block_getters.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/_contract_calls.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/_contract_calls.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/_mock_contract.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/_mock_contract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/interface_test.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/interface_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_interface.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_interface.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_interface_test.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_interface_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_write_interface.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_write_interface.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/interface/read_write_interface_test.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/interface/read_write_interface_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/receipt_breakdown.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/receipt_breakdown.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/state/pool_state.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/state/pool_state.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/hyperdrive/transactions.py` & `agent0-0.18.1/src/agent0/ethpy/hyperdrive/transactions.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/test_fixtures/deployed_pool.py` & `agent0-0.18.1/src/agent0/ethpy/test_fixtures/deployed_pool.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/test_fixtures/interface.py` & `agent0-0.18.1/src/agent0/ethpy/test_fixtures/interface.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/ethpy/test_fixtures/local_chain.py` & `agent0-0.18.1/src/agent0/ethpy/test_fixtures/local_chain.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hyperlogs/json_encoder.py` & `agent0-0.18.1/src/agent0/hyperlogs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hyperlogs/logs.py` & `agent0-0.18.1/src/agent0/hyperlogs/logs.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hyperlogs/logs_test.py` & `agent0-0.18.1/src/agent0/hyperlogs/logs_test.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hyperlogs/rollbar_utilities.py` & `agent0-0.18.1/src/agent0/hyperlogs/rollbar_utilities.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/README.md` & `agent0-0.18.1/src/agent0/hypertypes/README.md`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/fixedpoint_types.py` & `agent0-0.18.1/src/agent0/hypertypes/fixedpoint_types.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC20ForwarderFactoryContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC20ForwarderFactoryContract.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,15 +333,15 @@
             "stateMutability": "view",
         },
         {"type": "error", "name": "InvalidForwarderAddress", "inputs": []},
     ],
 )
 # pylint: disable=line-too-long
 erc20forwarderfactory_bytecode = HexStr(
-    "0x6080604052600080546001600160a01b0319166001908117909155805534801561002857600080fd5b50611441806100386000396000f3fe608060405234801561001057600080fd5b506004361061004c5760003560e01c80630710fd58146100515780630ecaea7314610081578063600eb4ba14610094578063d13053bb146100ca575b600080fd5b61006461005f3660046102cc565b6100e0565b6040516001600160a01b0390911681526020015b60405180910390f35b61006461008f3660046102cc565b6101b5565b6100ab6000546001546001600160a01b0390911691565b604080516001600160a01b039093168352602083019190915201610078565b6100d2610292565b604051908152602001610078565b604080516001600160a01b03841660208201529081018290526000908190606001604051602081830303815290604052805190602001209050600060ff60f81b308360405180602001610132906102bf565b6020820181038252601f19601f820116604052508051906020012060405160200161019494939291906001600160f81b031994909416845260609290921b6bffffffffffffffffffffffff191660018401526015830152603582015260550190565b60408051808303601f19018152919052805160209091012095945050505050565b6001819055600080546001600160a01b0319166001600160a01b038416908117825560408051602081019290925281018390528190606001604051602081830303815290604052805190602001209050600081604051610214906102bf565b8190604051809103906000f5905080158015610234573d6000803e3d6000fd5b50905061024185856100e0565b6001600160a01b0316816001600160a01b0316146102715760405162e0775560e61b815260040160405180910390fd5b600080546001600160a01b0319166001908117909155805591505092915050565b6040516102a1602082016102bf565b6020820181038252601f19601f820116604052508051906020012081565b6111078061030583390190565b600080604083850312156102df57600080fd5b82356001600160a01b03811681146102f657600080fd5b94602093909301359350505056fe60c060405234801561001057600080fd5b50604080516330075a5d60e11b815281513392839263600eb4ba92600480830193928290030181865afa15801561004b573d6000803e3d6000fd5b505050506040513d601f19601f8201168201806040525081019061006f9190610084565b60a0526001600160a01b0316608052506100be565b6000806040838503121561009757600080fd5b82516001600160a01b03811681146100ae57600080fd5b6020939093015192949293505050565b60805160a051610f9f610168600039600081816101400152818161028c015281816103400152818161043e015281816104e9015281816105fb015281816106b00152818161071f015281816109e40152610b8c015260008181610244015281816102b501528181610386015281816104670152818161053701528181610634015281816106d90152818161076f01528181610a2101528181610b020152610bca0152610f9f6000f3fe608060405234801561001057600080fd5b50600436106100f55760003560e01c806370a0823111610097578063d505accf11610066578063d505accf1461020f578063dd62ed3e14610224578063f698da2514610237578063fc0c546a1461023f57600080fd5b806370a08231146101c15780637ecebe00146101d457806395d89b41146101f4578063a9059cbb146101fc57600080fd5b806318160ddd116100d357806318160ddd1461017057806323b872dd1461017857806330adf81f1461018b578063313ce567146101b257600080fd5b806306fdde03146100fa578063095ea7b31461011857806317d70f7c1461013b575b600080fd5b61010261027e565b60405161010f9190610cee565b60405180910390f35b61012b610126366004610d3d565b610331565b604051901515815260200161010f565b6101627f000000000000000000000000000000000000000000000000000000000000000081565b60405190815260200161010f565b61016261042f565b61012b610186366004610d67565b6104da565b6101627f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c981565b6040516012815260200161010f565b6101626101cf366004610da3565b6105ec565b6101626101e2366004610da3565b60006020819052908152604090205481565b6101026106a1565b61012b61020a366004610d3d565b610710565b61022261021d366004610dc5565b61080a565b005b610162610232366004610e38565b610ad8565b610162610c3c565b6102667f000000000000000000000000000000000000000000000000000000000000000081565b6040516001600160a01b03909116815260200161010f565b604051622b600360e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201526060907f00000000000000000000000000000000000000000000000000000000000000006001600160a01b03169062ad800c906024015b600060405180830381865afa158015610304573d6000803e3d6000fd5b505050506040513d6000823e601f3d908101601f1916820160405261032c9190810190610e81565b905090565b6040516313b4b5ab60e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b038381166024830152604482018390523360648301526000917f000000000000000000000000000000000000000000000000000000000000000090911690634ed2d6ac90608401600060405180830381600087803b1580156103cc57600080fd5b505af11580156103e0573d6000803e3d6000fd5b50506040518481526001600160a01b03861692503391507f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b925906020015b60405180910390a35060015b92915050565b60405163bd85b03960e01b81527f000000000000000000000000000000000000000000000000000000000000000060048201526000907f00000000000000000000000000000000000000000000000000000000000000006001600160a01b03169063bd85b03990602401602060405180830381865afa1580156104b6573d6000803e3d6000fd5b505050506040513d601f19601f8201168201806040525081019061032c9190610f2e565b604051633912022f60e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b0384811660248301528381166044830152606482018390523360848301526000917f00000000000000000000000000000000000000000000000000000000000000009091169063e44808bc9060a401600060405180830381600087803b15801561057d57600080fd5b505af1158015610591573d6000803e3d6000fd5b50505050826001600160a01b0316846001600160a01b03167fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef846040516105da91815260200190565b60405180910390a35060019392505050565b604051631b2b776160e11b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b0382811660248301526000917f000000000000000000000000000000000000000000000000000000000000000090911690633656eec290604401602060405180830381865afa15801561067d573d6000803e3d6000fd5b505050506040513d601f19601f820116820180604052508101906104299190610f2e565b604051634e41a1fb60e01b81527f000000000000000000000000000000000000000000000000000000000000000060048201526060907f00000000000000000000000000000000000000000000000000000000000000006001600160a01b031690634e41a1fb906024016102e7565b604051633912022f60e21b81527f0000000000000000000000000000000000000000000000000000000000000000600482015233602482018190526001600160a01b0384811660448401526064830184905260848301919091526000917f00000000000000000000000000000000000000000000000000000000000000009091169063e44808bc9060a401600060405180830381600087803b1580156107b557600080fd5b505af11580156107c9573d6000803e3d6000fd5b50506040518481526001600160a01b03861692503391507fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef9060200161041d565b8342111561082b5760405163f87d927160e01b815260040160405180910390fd5b6001600160a01b0387166108525760405163f0dd15fd60e01b815260040160405180910390fd5b6001600160a01b03871660009081526020819052604081205490610874610c3c565b604080517f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c960208201526001600160a01b03808d1692820192909252908a1660608201526080810189905260a0810184905260c0810188905260e0016040516020818303038152906040528051906020012060405160200161090d92919061190160f01b81526002810192909252602282015260420190565b60408051601f198184030181528282528051602091820120600080855291840180845281905260ff89169284019290925260608301879052608083018690529092509060019060a0016020604051602081039080840390855afa158015610978573d6000803e3d6000fd5b505050602060405103519050896001600160a01b0316816001600160a01b0316146109b657604051638baa579f60e01b815260040160405180910390fd5b6001600160a01b03808b1660008181526020819052604090819020600187019055516313b4b5ab60e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201528b83166024820152604481018b905260648101919091527f000000000000000000000000000000000000000000000000000000000000000090911690634ed2d6ac90608401600060405180830381600087803b158015610a6757600080fd5b505af1158015610a7b573d6000803e3d6000fd5b50505050886001600160a01b03168a6001600160a01b03167f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9258a604051610ac491815260200190565b60405180910390a350505050505050505050565b60405163e985e9c560e01b81526001600160a01b03838116600483015282811660248301526000917f00000000000000000000000000000000000000000000000000000000000000009091169063e985e9c590604401602060405180830381865afa158015610b4b573d6000803e3d6000fd5b505050506040513d601f19601f82011682018060405250810190610b6f9190610f47565b15610b7d5750600019610429565b6040516321ff32a960e01b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b03848116602483015283811660448301527f000000000000000000000000000000000000000000000000000000000000000016906321ff32a990606401602060405180830381865afa158015610c11573d6000803e3d6000fd5b505050506040513d601f19601f82011682018060405250810190610c359190610f2e565b9050610429565b60408051808201825260018152603160f81b60209182015281517f2aef22f9d7df5f9d21c56d14029233f3fdaa91917727e1eb68e504d27072d6cd818301527fc89efdaa54c0f20c7adf612882df0950f5a951637e0307cdcb4c672f298b8bc681840152466060820152306080808301919091528351808303909101815260a0909101909252815191012090565b60005b83811015610ce5578181015183820152602001610ccd565b50506000910152565b6020815260008251806020840152610d0d816040850160208701610cca565b601f01601f19169190910160400192915050565b80356001600160a01b0381168114610d3857600080fd5b919050565b60008060408385031215610d5057600080fd5b610d5983610d21565b946020939093013593505050565b600080600060608486031215610d7c57600080fd5b610d8584610d21565b9250610d9360208501610d21565b9150604084013590509250925092565b600060208284031215610db557600080fd5b610dbe82610d21565b9392505050565b600080600080600080600060e0888a031215610de057600080fd5b610de988610d21565b9650610df760208901610d21565b95506040880135945060608801359350608088013560ff81168114610e1b57600080fd5b9699959850939692959460a0840135945060c09093013592915050565b60008060408385031215610e4b57600080fd5b610e5483610d21565b9150610e6260208401610d21565b90509250929050565b634e487b7160e01b600052604160045260246000fd5b600060208284031215610e9357600080fd5b815167ffffffffffffffff80821115610eab57600080fd5b818401915084601f830112610ebf57600080fd5b815181811115610ed157610ed1610e6b565b604051601f8201601f19908116603f01168101908382118183101715610ef957610ef9610e6b565b81604052828152876020848701011115610f1257600080fd5b610f23836020830160208801610cca565b979650505050505050565b600060208284031215610f4057600080fd5b5051919050565b600060208284031215610f5957600080fd5b81518015158114610dbe57600080fdfea2646970667358221220033f25da796c19d792c741eef3c9f1f265241835d5670c6054242d4ec7e8bf9864736f6c63430008140033a2646970667358221220e7e7c3e8b8fcffe83729f3edd7876600a93da978ce8dad0b6369f1fa28ea255064736f6c63430008140033"
+    "0x6080604052600080546001600160a01b0319166001908117909155805534801561002857600080fd5b50611441806100386000396000f3fe608060405234801561001057600080fd5b506004361061004c5760003560e01c80630710fd58146100515780630ecaea7314610081578063600eb4ba14610094578063d13053bb146100ca575b600080fd5b61006461005f3660046102cc565b6100e0565b6040516001600160a01b0390911681526020015b60405180910390f35b61006461008f3660046102cc565b6101b5565b6100ab6000546001546001600160a01b0390911691565b604080516001600160a01b039093168352602083019190915201610078565b6100d2610292565b604051908152602001610078565b604080516001600160a01b03841660208201529081018290526000908190606001604051602081830303815290604052805190602001209050600060ff60f81b308360405180602001610132906102bf565b6020820181038252601f19601f820116604052508051906020012060405160200161019494939291906001600160f81b031994909416845260609290921b6bffffffffffffffffffffffff191660018401526015830152603582015260550190565b60408051808303601f19018152919052805160209091012095945050505050565b6001819055600080546001600160a01b0319166001600160a01b038416908117825560408051602081019290925281018390528190606001604051602081830303815290604052805190602001209050600081604051610214906102bf565b8190604051809103906000f5905080158015610234573d6000803e3d6000fd5b50905061024185856100e0565b6001600160a01b0316816001600160a01b0316146102715760405162e0775560e61b815260040160405180910390fd5b600080546001600160a01b0319166001908117909155805591505092915050565b6040516102a1602082016102bf565b6020820181038252601f19601f820116604052508051906020012081565b6111078061030583390190565b600080604083850312156102df57600080fd5b82356001600160a01b03811681146102f657600080fd5b94602093909301359350505056fe60c060405234801561001057600080fd5b50604080516330075a5d60e11b815281513392839263600eb4ba92600480830193928290030181865afa15801561004b573d6000803e3d6000fd5b505050506040513d601f19601f8201168201806040525081019061006f9190610084565b60a0526001600160a01b0316608052506100be565b6000806040838503121561009757600080fd5b82516001600160a01b03811681146100ae57600080fd5b6020939093015192949293505050565b60805160a051610f9f610168600039600081816101400152818161028c015281816103400152818161043e015281816104e9015281816105fb015281816106b00152818161071f015281816109e40152610b8c015260008181610244015281816102b501528181610386015281816104670152818161053701528181610634015281816106d90152818161076f01528181610a2101528181610b020152610bca0152610f9f6000f3fe608060405234801561001057600080fd5b50600436106100f55760003560e01c806370a0823111610097578063d505accf11610066578063d505accf1461020f578063dd62ed3e14610224578063f698da2514610237578063fc0c546a1461023f57600080fd5b806370a08231146101c15780637ecebe00146101d457806395d89b41146101f4578063a9059cbb146101fc57600080fd5b806318160ddd116100d357806318160ddd1461017057806323b872dd1461017857806330adf81f1461018b578063313ce567146101b257600080fd5b806306fdde03146100fa578063095ea7b31461011857806317d70f7c1461013b575b600080fd5b61010261027e565b60405161010f9190610cee565b60405180910390f35b61012b610126366004610d3d565b610331565b604051901515815260200161010f565b6101627f000000000000000000000000000000000000000000000000000000000000000081565b60405190815260200161010f565b61016261042f565b61012b610186366004610d67565b6104da565b6101627f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c981565b6040516012815260200161010f565b6101626101cf366004610da3565b6105ec565b6101626101e2366004610da3565b60006020819052908152604090205481565b6101026106a1565b61012b61020a366004610d3d565b610710565b61022261021d366004610dc5565b61080a565b005b610162610232366004610e38565b610ad8565b610162610c3c565b6102667f000000000000000000000000000000000000000000000000000000000000000081565b6040516001600160a01b03909116815260200161010f565b604051622b600360e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201526060907f00000000000000000000000000000000000000000000000000000000000000006001600160a01b03169062ad800c906024015b600060405180830381865afa158015610304573d6000803e3d6000fd5b505050506040513d6000823e601f3d908101601f1916820160405261032c9190810190610e81565b905090565b6040516313b4b5ab60e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b038381166024830152604482018390523360648301526000917f000000000000000000000000000000000000000000000000000000000000000090911690634ed2d6ac90608401600060405180830381600087803b1580156103cc57600080fd5b505af11580156103e0573d6000803e3d6000fd5b50506040518481526001600160a01b03861692503391507f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b925906020015b60405180910390a35060015b92915050565b60405163bd85b03960e01b81527f000000000000000000000000000000000000000000000000000000000000000060048201526000907f00000000000000000000000000000000000000000000000000000000000000006001600160a01b03169063bd85b03990602401602060405180830381865afa1580156104b6573d6000803e3d6000fd5b505050506040513d601f19601f8201168201806040525081019061032c9190610f2e565b604051633912022f60e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b0384811660248301528381166044830152606482018390523360848301526000917f00000000000000000000000000000000000000000000000000000000000000009091169063e44808bc9060a401600060405180830381600087803b15801561057d57600080fd5b505af1158015610591573d6000803e3d6000fd5b50505050826001600160a01b0316846001600160a01b03167fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef846040516105da91815260200190565b60405180910390a35060019392505050565b604051631b2b776160e11b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b0382811660248301526000917f000000000000000000000000000000000000000000000000000000000000000090911690633656eec290604401602060405180830381865afa15801561067d573d6000803e3d6000fd5b505050506040513d601f19601f820116820180604052508101906104299190610f2e565b604051634e41a1fb60e01b81527f000000000000000000000000000000000000000000000000000000000000000060048201526060907f00000000000000000000000000000000000000000000000000000000000000006001600160a01b031690634e41a1fb906024016102e7565b604051633912022f60e21b81527f0000000000000000000000000000000000000000000000000000000000000000600482015233602482018190526001600160a01b0384811660448401526064830184905260848301919091526000917f00000000000000000000000000000000000000000000000000000000000000009091169063e44808bc9060a401600060405180830381600087803b1580156107b557600080fd5b505af11580156107c9573d6000803e3d6000fd5b50506040518481526001600160a01b03861692503391507fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef9060200161041d565b8342111561082b5760405163f87d927160e01b815260040160405180910390fd5b6001600160a01b0387166108525760405163f0dd15fd60e01b815260040160405180910390fd5b6001600160a01b03871660009081526020819052604081205490610874610c3c565b604080517f6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c960208201526001600160a01b03808d1692820192909252908a1660608201526080810189905260a0810184905260c0810188905260e0016040516020818303038152906040528051906020012060405160200161090d92919061190160f01b81526002810192909252602282015260420190565b60408051601f198184030181528282528051602091820120600080855291840180845281905260ff89169284019290925260608301879052608083018690529092509060019060a0016020604051602081039080840390855afa158015610978573d6000803e3d6000fd5b505050602060405103519050896001600160a01b0316816001600160a01b0316146109b657604051638baa579f60e01b815260040160405180910390fd5b6001600160a01b03808b1660008181526020819052604090819020600187019055516313b4b5ab60e21b81527f000000000000000000000000000000000000000000000000000000000000000060048201528b83166024820152604481018b905260648101919091527f000000000000000000000000000000000000000000000000000000000000000090911690634ed2d6ac90608401600060405180830381600087803b158015610a6757600080fd5b505af1158015610a7b573d6000803e3d6000fd5b50505050886001600160a01b03168a6001600160a01b03167f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9258a604051610ac491815260200190565b60405180910390a350505050505050505050565b60405163e985e9c560e01b81526001600160a01b03838116600483015282811660248301526000917f00000000000000000000000000000000000000000000000000000000000000009091169063e985e9c590604401602060405180830381865afa158015610b4b573d6000803e3d6000fd5b505050506040513d601f19601f82011682018060405250810190610b6f9190610f47565b15610b7d5750600019610429565b6040516321ff32a960e01b81527f000000000000000000000000000000000000000000000000000000000000000060048201526001600160a01b03848116602483015283811660448301527f000000000000000000000000000000000000000000000000000000000000000016906321ff32a990606401602060405180830381865afa158015610c11573d6000803e3d6000fd5b505050506040513d601f19601f82011682018060405250810190610c359190610f2e565b9050610429565b60408051808201825260018152603160f81b60209182015281517f2aef22f9d7df5f9d21c56d14029233f3fdaa91917727e1eb68e504d27072d6cd818301527fc89efdaa54c0f20c7adf612882df0950f5a951637e0307cdcb4c672f298b8bc681840152466060820152306080808301919091528351808303909101815260a0909101909252815191012090565b60005b83811015610ce5578181015183820152602001610ccd565b50506000910152565b6020815260008251806020840152610d0d816040850160208701610cca565b601f01601f19169190910160400192915050565b80356001600160a01b0381168114610d3857600080fd5b919050565b60008060408385031215610d5057600080fd5b610d5983610d21565b946020939093013593505050565b600080600060608486031215610d7c57600080fd5b610d8584610d21565b9250610d9360208501610d21565b9150604084013590509250925092565b600060208284031215610db557600080fd5b610dbe82610d21565b9392505050565b600080600080600080600060e0888a031215610de057600080fd5b610de988610d21565b9650610df760208901610d21565b95506040880135945060608801359350608088013560ff81168114610e1b57600080fd5b9699959850939692959460a0840135945060c09093013592915050565b60008060408385031215610e4b57600080fd5b610e5483610d21565b9150610e6260208401610d21565b90509250929050565b634e487b7160e01b600052604160045260246000fd5b600060208284031215610e9357600080fd5b815167ffffffffffffffff80821115610eab57600080fd5b818401915084601f830112610ebf57600080fd5b815181811115610ed157610ed1610e6b565b604051601f8201601f19908116603f01168101908382118183101715610ef957610ef9610e6b565b81604052828152876020848701011115610f1257600080fd5b610f23836020830160208801610cca565b979650505050505050565b600060208284031215610f4057600080fd5b5051919050565b600060208284031215610f5957600080fd5b81518015158114610dbe57600080fdfea2646970667358221220033f25da796c19d792c741eef3c9f1f265241835d5670c6054242d4ec7e8bf9864736f6c63430008140033a2646970667358221220801fb322ed362ba55c47b16836318792670f289cebd448fc5d025502942dfef764736f6c63430008140033"
 )
 
 
 class ERC20ForwarderFactoryContract(Contract):
     """A web3.py Contract class for the ERC20ForwarderFactory contract."""
 
     abi: ABI = erc20forwarderfactory_abi
```

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC20MintableContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC20MintableContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC20MintableTypes.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC20MintableTypes.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC4626HyperdriveCoreDeployerContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC4626HyperdriveCoreDeployerContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC4626HyperdriveDeployerCoordinatorContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC4626HyperdriveDeployerCoordinatorContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target0DeployerContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target0DeployerContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target1DeployerContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target1DeployerContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target2DeployerContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target2DeployerContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target3DeployerContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target3DeployerContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/ERC4626Target4DeployerContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/ERC4626Target4DeployerContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/HyperdriveDeployerCoordinatorTypes.py` & `agent0-0.18.1/src/agent0/hypertypes/types/HyperdriveDeployerCoordinatorTypes.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/HyperdriveFactoryContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/HyperdriveFactoryContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/HyperdriveFactoryTypes.py` & `agent0-0.18.1/src/agent0/hypertypes/types/HyperdriveFactoryTypes.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/IHyperdriveContract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/IHyperdriveContract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/IHyperdriveTypes.py` & `agent0-0.18.1/src/agent0/hypertypes/types/IHyperdriveTypes.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/MockERC4626Contract.py` & `agent0-0.18.1/src/agent0/hypertypes/types/MockERC4626Contract.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/MockERC4626Types.py` & `agent0-0.18.1/src/agent0/hypertypes/types/MockERC4626Types.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/__init__.py` & `agent0-0.18.1/src/agent0/hypertypes/types/__init__.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/types/utilities.py` & `agent0-0.18.1/src/agent0/hypertypes/types/utilities.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/hypertypes/utilities/conversions.py` & `agent0-0.18.1/src/agent0/hypertypes/utilities/conversions.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/traiderdaive/__init__.py` & `agent0-0.18.1/src/agent0/traiderdaive/__init__.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/traiderdaive/gym_environments/full_hyperdrive_env.py` & `agent0-0.18.1/src/agent0/traiderdaive/gym_environments/full_hyperdrive_env.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/src/agent0/traiderdaive/gym_environments/simple_hyperdrive_env.py` & `agent0-0.18.1/src/agent0/traiderdaive/gym_environments/simple_hyperdrive_env.py`

 * *Files identical despite different names*

### Comparing `agent0-0.18.0/PKG-INFO` & `agent0-0.18.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: agent0
-Version: 0.18.0
+Version: 0.18.1
 Summary: Agent interface for on-chain protocols.
 Author-email: Dylan Paiton <dylan@delv.tech>, Mihai Cosma <mihai@delv.tech>, Matthew Brown <matt@delv.tech>, Sheng Lundquist <sheng@delv.tech>, Jonny Rhea <jonny@delv.tech>, Alex Towle <alex@delv.tech>, Giovanni Effio <mazygio@delv.tech>, Ryan Goree <ryan@delv.tech>
 Requires-Python: >=3.10, <=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Requires-Dist: dill
 Requires-Dist: docker
+Requires-Dist: eth-typing==4.1.0
 Requires-Dist: fixedpointmath
 Requires-Dist: flask
 Requires-Dist: flask-expects-json
 Requires-Dist: hexbytes
-Requires-Dist: hyperdrivepy==0.13.0
+Requires-Dist: hyperdrivepy==1.0.1
 Requires-Dist: ipython
 Requires-Dist: matplotlib
 Requires-Dist: mplfinance
 Requires-Dist: nest_asyncio
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pandas-stubs
```

#### html2text {}

```diff
@@ -1,60 +1,60 @@
-Metadata-Version: 2.1 Name: agent0 Version: 0.18.0 Summary: Agent interface for
+Metadata-Version: 2.1 Name: agent0 Version: 0.18.1 Summary: Agent interface for
 on-chain protocols. Author-email: Dylan Paiton
 delv.tech>, Mihai Cosma
 delv.tech>, Matthew Brown
 delv.tech>, Sheng Lundquist
 delv.tech>, Jonny Rhea
 delv.tech>, Alex Towle
 delv.tech>, Giovanni Effio
 delv.tech>, Ryan Goree
 delv.tech> Requires-Python: >=3.10, <=3.11 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Development Status :: 3 - Alpha Classifier: Natural
 Language :: English Requires-Dist: dill Requires-Dist: docker Requires-Dist:
-fixedpointmath Requires-Dist: flask Requires-Dist: flask-expects-json Requires-
-Dist: hexbytes Requires-Dist: hyperdrivepy==0.13.0 Requires-Dist: ipython
-Requires-Dist: matplotlib Requires-Dist: mplfinance Requires-Dist: nest_asyncio
-Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: pandas-stubs
-Requires-Dist: psycopg[binary] Requires-Dist: pytest Requires-Dist: python-
-dotenv Requires-Dist: requests Requires-Dist: rollbar Requires-Dist: setuptools
-Requires-Dist: sqlalchemy Requires-Dist: sqlalchemy-utils Requires-Dist:
-streamlit Requires-Dist: web3 Requires-Dist: gymnasium ; extra == "ai"
-Requires-Dist: scipy ; extra == "ai" Requires-Dist: agent0[dev,ai,rollbar] ;
-extra == "all" Requires-Dist: autodocsumm>=0.2.11 ; extra == "dev" Requires-
-Dist: black==24.* ; extra == "dev" Requires-Dist: coverage ; extra == "dev"
-Requires-Dist: ipykernel ; extra == "dev" Requires-Dist: jupytext ; extra ==
-"dev" Requires-Dist: myst-parser>=2.0.0 ; extra == "dev" Requires-Dist:
-nbconvert ; extra == "dev" Requires-Dist: nbsphinx>=0.8.12 ; extra == "dev"
-Requires-Dist: numpydoc>=1.5.0 ; extra == "dev" Requires-Dist: pylint ; extra
-== "dev" Requires-Dist: pypechain ; extra == "dev" Requires-Dist: pytest-
-postgresql ; extra == "dev" Requires-Dist: pyright ; extra == "dev" Requires-
-Dist: sphinx>=6 ; extra == "dev" Requires-Dist: sphinx-autoapi>=2.0.1 ; extra
-== "dev" Requires-Dist: sphinx_autodoc_typehints>=1.21.8 ; extra == "dev"
-Requires-Dist: sphinx-rtd-theme>=1.2.2 ; extra == "dev" Requires-Dist:
-sphinxcontrib-napoleon>=0.7 ; extra == "dev" Requires-Dist: tomli>=2.0.1 ;
-extra == "dev" Requires-Dist: urllib3 ; extra == "dev" Requires-Dist: rollbar ;
-extra == "rollbar" Project-URL: Bug Tracker, https://github.com/delvtech/
-agent0/issues Project-URL: Homepage, https://agent0.readthedocs.io/en/latest/
-Provides-Extra: ai Provides-Extra: all Provides-Extra: dev Provides-Extra:
-rollbar [![linting: pylint](https://img.shields.io/badge/linting-pylint-
-yellowgreen)](https://github.com/pylint-dev/pylint) [![code style: black]
-(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) [![testing: pytest](https://img.shields.io/badge/testing-
-pytest-blue.svg)](https://docs.pytest.org/en/latest/contents.html) [![license:
-Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-lightgrey)](http://
-www.apache.org/licenses/LICENSE-2.0) [![DELV - Terms of Service](https://
-img.shields.io/badge/DELV-Terms_of_Service-orange)](https://elementfi.s3.us-
-east-2.amazonaws.com/element-finance-terms-of-service.pdf) [![testing:
-coverage](https://codecov.io/gh/delvtech/agent0/branch/main/graph/
-badge.svg?token=1S60MD42ZP)](https://app.codecov.io/gh/delvtech/
-agent0?displayType=list) [![docs: build](https://readthedocs.org/projects/
-agent0/badge/?version=latest)](https://agent0.readthedocs.io/en/latest/
-?badge=latest)
+eth-typing==4.1.0 Requires-Dist: fixedpointmath Requires-Dist: flask Requires-
+Dist: flask-expects-json Requires-Dist: hexbytes Requires-Dist:
+hyperdrivepy==1.0.1 Requires-Dist: ipython Requires-Dist: matplotlib Requires-
+Dist: mplfinance Requires-Dist: nest_asyncio Requires-Dist: numpy Requires-
+Dist: pandas Requires-Dist: pandas-stubs Requires-Dist: psycopg[binary]
+Requires-Dist: pytest Requires-Dist: python-dotenv Requires-Dist: requests
+Requires-Dist: rollbar Requires-Dist: setuptools Requires-Dist: sqlalchemy
+Requires-Dist: sqlalchemy-utils Requires-Dist: streamlit Requires-Dist: web3
+Requires-Dist: gymnasium ; extra == "ai" Requires-Dist: scipy ; extra == "ai"
+Requires-Dist: agent0[dev,ai,rollbar] ; extra == "all" Requires-Dist:
+autodocsumm>=0.2.11 ; extra == "dev" Requires-Dist: black==24.* ; extra ==
+"dev" Requires-Dist: coverage ; extra == "dev" Requires-Dist: ipykernel ; extra
+== "dev" Requires-Dist: jupytext ; extra == "dev" Requires-Dist: myst-
+parser>=2.0.0 ; extra == "dev" Requires-Dist: nbconvert ; extra == "dev"
+Requires-Dist: nbsphinx>=0.8.12 ; extra == "dev" Requires-Dist: numpydoc>=1.5.0
+; extra == "dev" Requires-Dist: pylint ; extra == "dev" Requires-Dist:
+pypechain ; extra == "dev" Requires-Dist: pytest-postgresql ; extra == "dev"
+Requires-Dist: pyright ; extra == "dev" Requires-Dist: sphinx>=6 ; extra ==
+"dev" Requires-Dist: sphinx-autoapi>=2.0.1 ; extra == "dev" Requires-Dist:
+sphinx_autodoc_typehints>=1.21.8 ; extra == "dev" Requires-Dist: sphinx-rtd-
+theme>=1.2.2 ; extra == "dev" Requires-Dist: sphinxcontrib-napoleon>=0.7 ;
+extra == "dev" Requires-Dist: tomli>=2.0.1 ; extra == "dev" Requires-Dist:
+urllib3 ; extra == "dev" Requires-Dist: rollbar ; extra == "rollbar" Project-
+URL: Bug Tracker, https://github.com/delvtech/agent0/issues Project-URL:
+Homepage, https://agent0.readthedocs.io/en/latest/ Provides-Extra: ai Provides-
+Extra: all Provides-Extra: dev Provides-Extra: rollbar [![linting: pylint]
+(https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/
+pylint-dev/pylint) [![code style: black](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black) [![testing:
+pytest](https://img.shields.io/badge/testing-pytest-blue.svg)](https://
+docs.pytest.org/en/latest/contents.html) [![license: Apache 2.0](https://
+img.shields.io/badge/License-Apache_2.0-lightgrey)](http://www.apache.org/
+licenses/LICENSE-2.0) [![DELV - Terms of Service](https://img.shields.io/badge/
+DELV-Terms_of_Service-orange)](https://elementfi.s3.us-east-2.amazonaws.com/
+element-finance-terms-of-service.pdf) [![testing: coverage](https://codecov.io/
+gh/delvtech/agent0/branch/main/graph/badge.svg?token=1S60MD42ZP)](https://
+app.codecov.io/gh/delvtech/agent0?displayType=list) [![docs: build](https://
+readthedocs.org/projects/agent0/badge/?version=latest)](https://
+agent0.readthedocs.io/en/latest/?badge=latest)
 _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_d_e_l_v_t_e_c_h_/_a_g_e_n_t_0_/_g_r_a_p_h_s_/_s_u_n_b_u_r_s_t_._s_v_g_?_t_o_k_e_n_=_1_S_6_0_M_D_4_2_Z_P_]
 _[_a_g_e_n_t_0_]
 _#_ _[_D_E_L_V_]_(_h_t_t_p_s_:_/_/_d_e_l_v_._t_e_c_h_)_ _r_e_p_o_ _f_o_r_ _m_a_r_k_e_t_ _s_i_m_u_l_a_t_i_o_n_ _a_n_d_ _a_n_a_l_y_s_i_s_ _T_h_i_s_ _d_o_c_s
 _p_a_g_e_ _c_a_n_ _b_e_ _f_o_u_n_d_ _v_i_a_ _[_h_t_t_p_s_:_/_/_a_g_e_n_t_0_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/_]_(_h_t_t_p_s_:_/_/
 _a_g_e_n_t_0_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_e_n_/_l_a_t_e_s_t_/_)_._ _#_#_ _Q_u_i_c_k_s_t_a_r_t_ _T_h_i_s_ _r_e_p_o_ _c_o_n_t_a_i_n_s_ _g_e_n_e_r_a_l
 _p_u_r_p_o_s_e_ _c_o_d_e_ _f_o_r_ _i_n_t_e_r_a_c_t_i_n_g_ _w_i_t_h_ _E_t_h_e_r_e_u_m_ _s_m_a_r_t_ _c_o_n_t_r_a_c_t_s_._ _H_o_w_e_v_e_r_,_ _i_t_ _w_a_s
 _b_u_l_i_t_ _f_o_r_ _t_h_e_ _p_r_i_m_a_r_y_ _u_s_e_ _c_a_s_e_ _o_f_ _t_r_a_d_i_n_g_ _o_n_ _[_H_y_p_e_r_d_r_i_v_e_]_(_h_t_t_p_s_:_/_/
```

