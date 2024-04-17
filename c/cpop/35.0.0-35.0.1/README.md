# Comparing `tmp/cpop-35.0.0.tar.gz` & `tmp/cpop-35.0.1.tar.gz`

## Comparing `cpop-35.0.0.tar` & `cpop-35.0.1.tar`

### file list

```diff
@@ -1,176 +1,175 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-35.0.0/.coveragerc
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 cpop-35.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/Makefile
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/make.bat
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/outline.rst
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/releases/32.rst
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/app_merging.rst
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/conf.rst
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/conf_integrate.rst
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/contracts.rst
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/dyne_name.rst
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/func_alias.rst
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/glossary.rst
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/hub_overview.rst
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/ideas_that_were_not_used.rst
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/learning.rst
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/pop.rst
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/pre_contract_returns.rst
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/story.rst
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/sub_patterns.rst
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/subs_overview.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/topics/virtual.rst
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.0.0/docs/source/tutorial/quickstart.rst
--rw-r--r--   0        0        0     9659 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/data.pyx
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/dirs.pyx
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/exc.pyx
--rw-r--r--   0        0        0    26634 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/hub.pyx
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/loader.pyx
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/ref.pyx
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/scanner.pyx
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.0.0/src/cpop/verify.pyx
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/config.yaml
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/log/basic.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/log/init.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/log/timed_rolling.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/log/contracts/init.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/mods/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-35.0.0/src/pop/mods/test.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/contracts/test.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/coro/contracts/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_cli.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_config.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_cpop.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_dyne.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_hub.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_log.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_ref.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/proc.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/vtrue.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.0.0/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.0.0/.gitignore
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 cpop-35.0.0/README.rst
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 cpop-35.0.0/pyproject.toml
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 cpop-35.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/Makefile
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/make.bat
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/outline.rst
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/releases/32.rst
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/app_merging.rst
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/conf.rst
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/conf_integrate.rst
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/contracts.rst
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/dyne_name.rst
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/func_alias.rst
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/glossary.rst
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/hub_overview.rst
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/ideas_that_were_not_used.rst
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/learning.rst
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/pop.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/pre_contract_returns.rst
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/story.rst
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/sub_patterns.rst
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/subs_overview.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/virtual.rst
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/tutorial/quickstart.rst
+-rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/data.pyx
+-rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/dirs.pyx
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/exc.pyx
+-rw-r--r--   0        0        0    26676 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/hub.pyx
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/loader.pyx
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/ref.pyx
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/scanner.pyx
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/verify.pyx
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/config.yaml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/basic.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/init.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/config.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/test.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_ref.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/proc.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.0.1/.gitignore
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 cpop-35.0.1/README.rst
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cpop-35.0.1/PKG-INFO
```

### Comparing `cpop-35.0.0/.pre-commit-config.yaml` & `cpop-35.0.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -38,20 +38,14 @@
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.2
     hooks:
       - id: pyupgrade
         name: Rewrite Code to be Py3.10+
         args: [--py310-plus]
 
-  - repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.12.0
-    hooks:
-      - id: reorder-python-imports
-        args: [--py310-plus]
-
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         types: [yaml, toml]
 
   - repo: https://github.com/myint/rstcheck
@@ -63,23 +57,26 @@
         additional_dependencies: [sphinx]
 
   - repo: local
     hooks:
       - id: hatch-fmt
         name: Format code with hatch fmt
         entry: hatch fmt
-        language: system
+        language: python
         pass_filenames: false
         verbose: true
+        additional_dependencies:
+          - hatch
+          - hatch-cython
 
   - repo: https://github.com/MarcoGorelli/cython-lint
     rev: v0.16.0
     hooks:
-    -   id: cython-lint
-    -   id: double-quote-cython-strings
+      - id: cython-lint
+      - id: double-quote-cython-strings
 
   # <---- Formatting -----------------------------------------------------------------------------
 
   # ----- Security -------------------------------------------------------------------------------------------------->
   - repo: https://github.com/PyCQA/bandit
     rev: "1.7.8"
     hooks:
```

### Comparing `cpop-35.0.0/docs/Makefile` & `cpop-35.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/make.bat` & `cpop-35.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/outline.rst` & `cpop-35.0.1/docs/outline.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/conf.py` & `cpop-35.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/index.rst` & `cpop-35.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/app_merging.rst` & `cpop-35.0.1/docs/source/topics/app_merging.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/conf.rst` & `cpop-35.0.1/docs/source/topics/conf.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/conf_integrate.rst` & `cpop-35.0.1/docs/source/topics/conf_integrate.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/contracts.rst` & `cpop-35.0.1/docs/source/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/dyne_name.rst` & `cpop-35.0.1/docs/source/topics/dyne_name.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/func_alias.rst` & `cpop-35.0.1/docs/source/topics/func_alias.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/glossary.rst` & `cpop-35.0.1/docs/source/topics/glossary.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/hub_overview.rst` & `cpop-35.0.1/docs/source/topics/hub_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/ideas_that_were_not_used.rst` & `cpop-35.0.1/docs/source/topics/ideas_that_were_not_used.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/learning.rst` & `cpop-35.0.1/docs/source/topics/learning.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/pop.rst` & `cpop-35.0.1/docs/source/topics/pop.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/pre_contract_returns.rst` & `cpop-35.0.1/docs/source/topics/pre_contract_returns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/story.rst` & `cpop-35.0.1/docs/source/topics/story.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/sub_patterns.rst` & `cpop-35.0.1/docs/source/topics/sub_patterns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/subs_overview.rst` & `cpop-35.0.1/docs/source/topics/subs_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/topics/virtual.rst` & `cpop-35.0.1/docs/source/topics/virtual.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/docs/source/tutorial/quickstart.rst` & `cpop-35.0.1/docs/source/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/cpop/contract.pyx` & `cpop-35.0.1/src/cpop/contract.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import asyncio
 import inspect
 import sys
 import traceback
 from collections.abc import Iterable
-from collections.abc import Mapping
 from cpython cimport dict
-from cython cimport pint
-from cpython.ref cimport PyObject
 
 cdef class ContractedContext:
     """
     Contracted function calling context
     """
     cdef:
         public object func
@@ -94,14 +91,15 @@
         cnames = getattr(mod, "__contracts__")
         for cname in cnames:
             if cname in contracts:
                 loaded_contracts.append(cname)
                 raws.append(getattr(contracts, cname))
     return raws
 
+
 cdef class Contracted:
     """
     This class wraps functions that have a contract associated with them
     and executes the contract routines
     """
     cdef:
         public bint _has_contracts
@@ -112,16 +110,15 @@
         public object signature
         public str __name__
         public str ref
         list _sig_errors
         list contracts
         object __wrapped__
 
-
-    def __init__(self, hub, contracts:list, func:object, ref:str, name:str, implicit_hub:bool=True):
+    def __init__(self, hub, contracts: list, func: object, ref: str, name: str, implicit_hub: bool = True):
         self.__name__ = name
         self.__wrapped__ = func
         self._sig_errors = []
         self.contracts = contracts or []
         self.func = func
         self.hub = hub
         self.implicit_hub = implicit_hub
@@ -135,15 +132,15 @@
     def __signature__(self):
         return self.signature
 
     @property
     def __dict__(self):
         return self.func.__dict__
 
-    cdef _get_contracts_by_type(self, contract_type:str):
+    cdef _get_contracts_by_type(self, contract_type: str):
         matches = []
         fn_contract_name = f"{contract_type}_{self.__name__}"
         for contract in self.contracts:
             if hasattr(contract, fn_contract_name):
                 matches.append(getattr(contract, fn_contract_name))
             if hasattr(contract, contract_type):
                 matches.append(getattr(contract, contract_type))
@@ -158,15 +155,15 @@
         # if ContractedAsync - allow coroutines and functions
 
         self.contract_functions = {
             "pre": self._get_contracts_by_type("pre"),
             "call": self._get_contracts_by_type("call")[:1],
             "post": self._get_contracts_by_type("post"),
         }
-        self._has_contracts = sum(len(l) for l in self.contract_functions.values()) > 0
+        self._has_contracts = sum(len(funcs) for funcs in self.contract_functions.values()) > 0
 
     async def __call__(self, *args, **kwargs):
         async with CallStack(self):
             if self.implicit_hub:
                 args = (self.hub,) + args
 
             if not self._has_contracts:
@@ -206,26 +203,25 @@
         return {
             "ref": self.ref,
             "name": self.__name__,
             "implicit_hub": self.implicit_hub,
             "contracts": self.contracts,
         }
 
-    def __setstate__(self, state:dict[str, object]):
+    def __setstate__(self, state: dict[str, object]):
         self.ref = state["ref"]
         self.__name__ = state["name"]
         self.func = self.hub[self.ref][self.__name__].func
         self.implicit_hub = state["implicit_hub"]
         self.contracts = state["contracts"]
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.ref}.{self.__name__}>"
 
 
-
 class ContractedAsyncGen(Contracted):
     async def __call__(self, *args, **kwargs):
         async with CallStack(self):
             if self.implicit_hub:
                 args = (self.hub,) + args
 
             if not self._has_contracts:
@@ -252,14 +248,15 @@
             ret = chunk
             for fn in self.contract_functions["post"]:
                 contract_context.ret = ret
                 post_ret = await fn(contract_context)
                 if post_ret is not None:
                     ret = post_ret
 
+
 class CallStack:
     """
     A wrapper for functions to add and remove their context from the stack securely
     """
     def __init__(self, contract: Contracted):
         self.contract = contract
```

### Comparing `cpop-35.0.0/src/cpop/data.pyx` & `cpop-35.0.1/src/cpop/data.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # cython: language_level=3
 
 from collections.abc import Mapping
 from cpython cimport dict
-from cython cimport pint
-from cpython.ref cimport PyObject
 
 
 cdef frozenset DICT_ATTRS = frozenset(dir(dict))
 
 cdef class NamespaceDict(dict[str, object]):
     def __getattr__(self, key: str):
         if key.startswith("__") and key.endswith("__"):
@@ -35,15 +33,15 @@
         self._cache = dict[str, object]()
         self._split_cache = dict[str, list[str]]()
 
     cpdef _clear(self):
         self._cache.clear()
         self._split_cache.clear()
 
-    def __getitem__(self, key:str):
+    def __getitem__(self, key: str):
         if key in self._cache:
             return self._cache[key]
 
         if key not in self._split_cache:
             self._split_cache[key] = key.split(".")
 
         parts = self._split_cache[key]
@@ -148,14 +146,15 @@
     elif isinstance(data, list):
         return tuple(freeze(value) for value in data)
     elif isinstance(data, set):
         return frozenset(freeze(value) for value in data)
     else:
         return data
 
+
 def unfreeze(data):
     if isinstance(data, ImmutableNamespaceDict):
         return {key: unfreeze(value) for key, value in data.items()}
     elif isinstance(data, frozenset):
         return {unfreeze(value) for value in data}
     elif isinstance(data, tuple):
         return [unfreeze(value) for value in data]
```

### Comparing `cpop-35.0.0/src/cpop/dirs.pyx` & `cpop-35.0.1/src/cpop/dirs.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import importlib.resources
 import os
 import aiopath
 import sys
 from collections import defaultdict
 from collections.abc import Iterable
-from typing import Any
 
 import cpop.data
 import msgpack
 import yaml
 
 
 async def dir_list(pypath: list[str] = None, static: list[str] = None) -> list[aiopath.Path]:
```

### Comparing `cpop-35.0.0/src/cpop/exc.pyx` & `cpop-35.0.1/src/cpop/exc.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/cpop/hub.pyx` & `cpop-35.0.1/src/cpop/hub.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,18 @@
     if isinstance(path, str):
         return path.split(",")
     elif isinstance(path, list):
         return path
     else:
         return []
 
+
 SHUTDOWN_SIGNAL = object()
+
+
 class PopMeta(cpop.data.MultidictCache):
     _subs = None
 
     def __init__(self, data: list[dict[str, any]]):
         attrs = {}
         data.append(attrs)
         super().__init__(data)
@@ -49,15 +52,15 @@
             for p in parts[:-1]:
                 if not p:
                     continue
                 if p not in finder:
                     finder[p] = cpop.data.NamespaceDict()
                 finder = finder[p]
 
-            finder[parts[len(parts) -1 ]] = value
+            finder[parts[len(parts)-1]] = value
         else:
             self._attrs[key] = value
 
     def __setattr__(self, key: str, value):
         if key.startswith("_"):
             object.__setattr__(self, key, value)
         else:
@@ -68,25 +71,26 @@
 class Hub(PopMeta):
     """
     The redistributed pop central hub. All components of the system are
     rooted to the Hub.
     """
     _call_stack = ContextVar("_call_stack", default=[])
 
-    def __init__(self, 
-        load_all_dynes: bool = True,
-        load_all_subdirs: bool = True,
-        recurse_subdirs: bool = True,
-        pop_mods: list[str] = None,
-        cli: str = None,
-        logs: bool = True,
-        load_config: bool = True,
-        sigint = None,
-        sigterm = None,
-    ):        
+    def __init__(
+            self,
+            load_all_dynes: bool = True,
+            load_all_subdirs: bool = True,
+            recurse_subdirs: bool = True,
+            pop_mods: list[str] = None,
+            cli: str = None,
+            logs: bool = True,
+            load_config: bool = True,
+            sigint = None,
+            sigterm = None
+            ):
         self._init_kwargs = {
             k: v for k, v in locals().items() if k != "self" and not k.startswith("_")
         }
         subs = {}
         sub_alias = {}
         imports = {}
         PopMeta.__init__(self, [subs, sub_alias, imports])
@@ -137,15 +141,14 @@
 
             # Add the pop sub to the hub, this should always use pypath and
             # Should never be made dynamic. This is a core system sub and should
             # NOT be app-merged
             self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
             await self._subs["pop"]._load_all()
 
-
         self._load_all_dynes = self._init_kwargs["load_all_dynes"]
         self._load_all_subdirs = self._init_kwargs["load_all_subdirs"]
         self._recurse_subdirs = self._init_kwargs["recurse_subdirs"]
         if self._load_all_dynes:
             await self._scan_dynamic()
             await self._load_all()
 
@@ -155,17 +158,17 @@
 
         # Set up a logger
         if "log" in self._subs and self._init_kwargs["logs"]:
             await self.log.init.setup(**self._opt.log.copy())
 
         return self
 
-    async def __aexit__(self, exc_type, exc_value, traceback):
+    async def __aexit__(self, exc_type, exc_value, tb):
         if exc_type is not None and exc_value is not None:
-            self._traceback(exc_type, exc_value, traceback)
+            self._traceback(exc_type, exc_value, tb)
         await self._tasks.put(SHUTDOWN_SIGNAL)
 
     @property
     def OPT(self):
         return self._opt
 
     async def _load_all(self):
@@ -179,30 +182,28 @@
             await self.pop.sub.add(dyne_name=dyne)
             if not self._load_all_subdirs:
                 continue
             await self.pop.sub.load_subdirs(
                 self._subs[dyne], recurse=self._recurse_subdirs
             )
 
-
     async def _holder(self):
         """
         Just a sleeping while loop to hold the loop open while it runs until
         complete
         """
         while True:
             complete = await self._tasks.get()
             if complete is  SHUTDOWN_SIGNAL:
                 break
             await complete["task"]
             if complete["cb"]:
                 await self._auto(complete["cb"])
             self._task_count -= 1
 
-
     def _auto(self, coro, cb_coro=None):
         """
         Start a task that will be automatically awaited
 
         coro: An unscheduled coroutine object to run
         cb_coro: An unscheduled coroutine to run when the main coroutine completes
         """
@@ -223,25 +224,24 @@
             task.add_done_callback(_callback)
             return task
         finally:
             # Cleanup, reset the context when add_done_callback
             self._call_stack.reset(token)
 
     @classmethod
-    def _call_stack_push(cls, ref:str, stack_summary):
+    def _call_stack_push(cls, ref: str, stack_summary):
         stack = cls._call_stack.get()
         stack.append((ref, stack_summary))
 
     @classmethod
     def _call_stack_pop(cls):
         stack = cls._call_stack.get()
         if stack:
             stack.pop()
 
-
     def _traceback(self, exctype, value, tb):
         call_stack = self._call_stack.get()
         if call_stack:
             # Fetch the most recent call from the custom stack
             ref, stack = call_stack[len(call_stack) - 1]
             print(f"\nMost recent call from {ref}:", file=sys.stderr)
             # Get only the last frame in the most recent call
@@ -251,15 +251,14 @@
             if line:
                 print(f"    {line}", file=sys.stderr)
 
         # Print the standard traceback
         print("\nStandard exception traceback (most recent call last):", file=sys.stderr)
         traceback.print_exception(exctype, value, tb, limit=1, file=sys.stderr)
 
-
     def __getstate__(self) -> dict:
         attrs = {}
         for k, v in self._attrs.items():
             if isinstance(v, cpop.loader.BASE_TYPES):
                 attrs[k] = v
             elif isinstance(v, dict):
                 if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in v.values()):
@@ -370,15 +369,16 @@
         :param omit_end:Allows you to pass in a tuple of characters that would omit the loading of an object
             (You should probably never change this)
         :param omit_func: bool: Don't load any functions
         :param omit_class: bool: Don't load any classes
         :param omit_vars: bool: Don't load any vars
         :param mod_basename: str: Manipulate the location in sys.modules that the plugin will be loaded to.
             Allow plugins to be loaded into a separate namespace.
-        :param stop_on_failures: If any module fails to load for any reason, stacktrace and do not continue loading this sub
+        :param stop_on_failures: If any module fails to load for any reason, stacktrace and do not continue
+            loading this sub
         :param init: bool: determine whether or not we process __init__ functions
         :param is_contract: Specify whether or not this sub is a contract
         :param sub_virtual: bool: Recursively ignore this sub and it's subs
         """
         self._init_kwargs = {
             k: v
             for k, v in locals().items()
```

### Comparing `cpop-35.0.0/src/cpop/loader.pyx` & `cpop-35.0.1/src/cpop/loader.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import importlib.util
 import inspect
 import os
 import sys
 import types
 from collections.abc import Callable
 from typing import Any
-from typing import List
 from typing import Union
 
 import cpop.contract
 import cpop.data
 
 BASE_TYPES = (int, float, str, bytes, bool, type(None))
 
@@ -29,15 +28,14 @@
             "msg": msg,
             "exception": exception,
             "verror": verror,
         }
         self.traceback = traceback
 
 
-
 def load_mod(modname: str, form: str, path: str) -> "LoadedMod":
     """
     Load a single module
     :param modname: The name of the module to get from the loader
     :param form: The name of the loader module
     :param path: The package to use as the anchor point from which to resolve the
         relative import to an absolute import.
@@ -164,26 +162,26 @@
             name="__init__",
         )
         await init()
 
 
 def sub_alias(this_sub, mod: "LoadedMod", mod_name: str):
     """
-    Check the sub alias settings and apply the alias names locally so they can be gathered into the higher level object on the hub
+    Check the sub alias settings and apply the alias names locally so they can be gathered into the
+        higher level object on the hub
     :param this_sub: The pop object that contains the loaded module data
     :param mod: A loader module
     :param mod_name: The name of the module to get from the loader
     """
     if mod_name == "init":
         alias = getattr(mod, "__sub_alias__", None)
         if alias:
             this_sub._alias = alias
 
 
-
 async def prep_loaded_mod(
     this_sub,
     mod: "LoadedMod",
     mod_name: str,
     contracts: "List[cpop.contract.Wrapper]",
     recursive_contracts: "List[cpop.contract.Wrapper]",
 ) -> "LoadedMod":
@@ -210,15 +208,19 @@
         func_alias_dict.update(__func_alias__)
 
     for attr in getattr(mod, "__load__", dir(mod)):
         func_alias: Union[str, Callable] = func_alias_dict.get(attr, attr)
         func = getattr(mod, attr)
         name = func_alias if isinstance(func_alias, str) else attr
 
-        if not this_sub._omit_vars and not (inspect.isfunction(func) or inspect.isclass(func) or type(func).__name__ == "cython_function_or_method"):
+        if not this_sub._omit_vars and not (
+                    inspect.isfunction(func) or
+                    inspect.isclass(func) or
+                    type(func).__name__ == "cython_function_or_method"
+                ):
             setattr(lmod, name, func)
             continue
 
         if attr.startswith(tuple(this_sub._omit_start)) or attr.endswith(tuple(this_sub._omit_end)):
             continue
 
         if inspect.isfunction(func) or inspect.isbuiltin(func) or type(func).__name__ == "cython_function_or_method":
@@ -228,21 +230,29 @@
         elif not this_sub._omit_class and inspect.isclass(func) and func.__module__.startswith(mod.__name__):
             lmod._classes[name] = func
 
     for attr, func_alias in func_alias_dict.items():
         if isinstance(func_alias, cpop.contract.Contracted):
             obj = func_alias
         elif isinstance(func_alias, Callable):
-            obj = cpop.contract.create_contracted(this_sub._hub, ordered_contracts, func_alias, ref, attr, implicit_hub=False)
+            obj = cpop.contract.create_contracted(
+                this_sub._hub,
+                ordered_contracts,
+                func_alias,
+                ref,
+                attr,
+                implicit_hub=False
+            )
         else:
             continue
         lmod._funcs[attr] = obj
 
     return lmod
 
+
 class LoadedMod(types.ModuleType):
     """
     The LoadedMod class allows for the module loaded onto the sub to return
     custom sequencing, for instance it can be iterated over to return all
     functions
     """
```

### Comparing `cpop-35.0.0/src/cpop/ref.pyx` & `cpop-35.0.1/src/cpop/ref.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Used to resolve resolutions to paths on the hub
 """
 
+
 def last(hub, ref) -> object:
     """
     Takes a string that references the desired ref and returns the last object
     called out in that ref
     """
     refs = path(hub, ref)
     return refs.pop()
```

### Comparing `cpop-35.0.0/src/cpop/scanner.pyx` & `cpop-35.0.1/src/cpop/scanner.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/cpop/verify.pyx` & `cpop-35.0.1/src/cpop/verify.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/pop/config.yaml` & `cpop-35.0.1/src/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/pop/log/basic.py` & `cpop-35.0.1/src/pop/log/basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/pop/log/init.py` & `cpop-35.0.1/src/pop/log/init.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,28 +49,33 @@
     """
     Initialize the logger with the named plugin
     """
     if hub.log.HANDLER:
         # We already set up the logger
         return
 
+    # Set up trace logger
+    hub.lib.aiologger.levels.LEVEL_TO_NAME[5] = "TRACE"
+    levels = hub.lib.logging.getLevelNamesMapping()
+    levels["TRACE"] = 5
+    hub.lib.logging.addLevelName(5, "TRACE")
+
+    # Convert log level to integer
     if str(log_level).isdigit():
         hub.log.INT_LEVEL = int(log_level)
     else:
-        hub.lib.aiologger.levels.LEVEL_TO_NAME[5] = "TRACE"
-        levels = hub.lib.logging.getLevelNamesMapping()
-        levels["TRACE"] = 5
-        hub.lib.logging.addLevelName(5, "TRACE")
         hub.log.INT_LEVEL = levels[log_level.upper()]
 
     if log_plugin != "init":
+        # Create the log file
         if log_file:
             path = await hub.lib.aiopath.Path(log_file).expanduser()
-            if not await path.exists():
-                await path.mkdir(parents=True, exist_ok=True)
+            if not await path.parent.exists():
+                await path.parent.mkdir(parents=True, exist_ok=True)
+            await path.touch(exist_ok=True)
             log_file = str(path)
         await hub.log[log_plugin].setup(log_file=log_file, **kwargs)
 
 
 async def trace(hub, msg: str, *args, **kwargs):
     ref, lineno = await hub.log.init.get_caller()
     logger = await hub.log.init.get_logger(ref)
```

### Comparing `cpop-35.0.0/src/pop/log/timed_rolling.py` & `cpop-35.0.1/src/pop/log/timed_rolling.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/pop/mods/config.py` & `cpop-35.0.1/src/pop/mods/config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/pop/mods/contract.py` & `cpop-35.0.1/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/pop/mods/sub.py` & `cpop-35.0.1/src/pop/mods/sub.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,23 +176,22 @@
         sub = getattr(hub, subname)
         await sub._prepare()
         return True
     else:
         return False
 
 
-async def iter_subs(hub, sub, recurse: bool = False):
+async def iter_subs(hub, sub, *, recurse: bool = False):
     """
     Return an iterator that will traverse just the subs. This is useful for
     nested subs
     :param hub: The redistributed pop central hub
     :param recurse: Recursively iterate over nested subs
     """
     for name in sorted(sub._subs):
         ret = sub._subs[name]
         if ret._sub_virtual:
             yield ret
             if recurse:
                 if hasattr(ret, "_subs"):
-                    async for rsub in hub.pop.sub.iter_subs(ret, recurse):
+                    async for rsub in hub.pop.sub.iter_subs(ret, recurse=recurse):
                         yield rsub
-
```

### Comparing `cpop-35.0.0/src/pop/mods/task.py` & `cpop-35.0.1/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/src/pop/mods/test.py` & `cpop-35.0.1/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/conftest.py` & `cpop-35.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/contracts/ctx.py` & `cpop-35.0.1/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/contracts/many.py` & `cpop-35.0.1/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/contracts/test.py` & `cpop-35.0.1/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_basic.py` & `cpop-35.0.1/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_config.py` & `cpop-35.0.1/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_contract_ctx.py` & `cpop-35.0.1/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_fail.py` & `cpop-35.0.1/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_log.py` & `cpop-35.0.1/tests/func/test_log.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_no_raise_on_pre_failure.py` & `cpop-35.0.1/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_raise_on_pre_failure.py` & `cpop-35.0.1/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_ref.py` & `cpop-35.0.1/tests/func/test_ref.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/func/test_serial.py` & `cpop-35.0.1/tests/func/test_serial.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/mods/proc.py` & `cpop-35.0.1/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/mods/test.py` & `cpop-35.0.1/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/regression/contract_masking/test_contract_masking.py` & `cpop-35.0.1/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-35.0.1/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/tpath/cn/contract/test.py` & `cpop-35.0.1/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/unit/test_contract.py` & `cpop-35.0.1/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/tests/unit/test_sigs.py` & `cpop-35.0.1/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/.gitignore` & `cpop-35.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-35.0.0/README.rst` & `cpop-35.0.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     import asyncio
 
     loop = asyncio.get_event_loop()
     asyncio.run(main())
 
 
     async def main():
-        hub = await cpop.hub.AsyncHub()
-        await hub._loop_start(hub.my_sub.init.cli())
+        async with cpop.hub.Hub() as hub:
+            await hub.my_sub.init.cli()
 
 
 Configuration
 =============
 
 When creating a cpop app, we put all of the pop configuration in a config.yaml
```

### Comparing `cpop-35.0.0/pyproject.toml` & `cpop-35.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython", "hatch-compile-yaml>=18.0.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "35.0.0"
+version = "35.0.1"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
@@ -41,14 +41,15 @@
 
 build = [
     "Cython",
     "hatch",
     "hatch-cython",
 ]
 
+
 [tool.hatch.build.targets.wheel]
 packages = [
     "src/cpop",
     "src/pop",
 ]
 
 [tool.hatch.build.hooks.convert-data-file.options]
@@ -199,10 +200,10 @@
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 
 docstring-code-format = true
 docstring-code-line-length = "dynamic"
 
 [tool.cython-lint]
-max-line-length = 88
+max-line-length = 120
 ignore = [
 ]
```

### Comparing `cpop-35.0.0/PKG-INFO` & `cpop-35.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 35.0.0
+Version: 35.0.1
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -67,16 +67,16 @@
     import asyncio
 
     loop = asyncio.get_event_loop()
     asyncio.run(main())
 
 
     async def main():
-        hub = await cpop.hub.AsyncHub()
-        await hub._loop_start(hub.my_sub.init.cli())
+        async with cpop.hub.Hub() as hub:
+            await hub.my_sub.init.cli()
 
 
 Configuration
 =============
 
 When creating a cpop app, we put all of the pop configuration in a config.yaml
```

