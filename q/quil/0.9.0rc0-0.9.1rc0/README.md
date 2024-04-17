# Comparing `tmp/quil-0.9.0rc0.tar.gz` & `tmp/quil-0.9.1rc0.tar.gz`

## Comparing `quil-0.9.0rc0.tar` & `quil-0.9.1rc0.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0     1001      127     1419 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/Cargo.toml
--rw-r--r--   0     1001      127    44103 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/CHANGELOG.md
--rw-r--r--   0     1001      127      954 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/README.md
--rw-r--r--   0     1001      127     1692 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/corpus.rs
--rw-r--r--   0     1001      127      941 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/get_frames_for_instruction.rs
--rw-r--r--   0     1001      127      985 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/parser.rs
--rw-r--r--   0     1001      127   803952 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/sample-calibrations.quil
--rw-r--r--   0     1001      127     1478 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/scheduled_program_from_program.rs
--rw-r--r--   0     1001      127      969 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/simplification.rs
--rw-r--r--   0     1001      127    12979 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/test_expressions.txt
--rw-r--r--   0     1001      127     6316 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/examples/generate_test_expressions.rs
--rw-r--r--   0     1001      127    38082 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/expression/mod.rs
--rw-r--r--   0     1001      127    34338 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/expression/simplification/by_hand.rs
--rw-r--r--   0     1001      127    12745 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/expression/simplification/mod.rs
--rw-r--r--   0     1001      127     1002 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/hash.rs
--rw-r--r--   0     1001      127     5302 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     6478 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/circuit.rs
--rw-r--r--   0     1001      127     9937 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/classical.rs
--rw-r--r--   0     1001      127     5260 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     6939 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9842 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/frame.rs
--rw-r--r--   0     1001      127    43954 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/gate.rs
--rw-r--r--   0     1001      127      771 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/measurement.rs
--rw-r--r--   0     1001      127    39443 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1798 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/pragma.rs
--rw-r--r--   0     1001      127     3425 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      654 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/reset.rs
--rw-r--r--   0     1001      127      133 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
--rw-r--r--   0     1001      127      133 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
--rw-r--r--   0     1001      127      124 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
--rw-r--r--   0     1001      127      167 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
--rw-r--r--   0     1001      127      160 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
--rw-r--r--   0     1001      127      109 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
--rw-r--r--   0     1001      127      141 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
--rw-r--r--   0     1001      127      125 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
--rw-r--r--   0     1001      127      191 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
--rw-r--r--   0     1001      127      178 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
--rw-r--r--   0     1001      127      139 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
--rw-r--r--   0     1001      127      143 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
--rw-r--r--   0     1001      127     1528 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/timing.rs
--rw-r--r--   0     1001      127     3666 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1910 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/lib.rs
--rw-r--r--   0     1001      127     1013 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/macros.rs
--rw-r--r--   0     1001      127    36217 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/command.rs
--rw-r--r--   0     1001      127    23080 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/common.rs
--rw-r--r--   0     1001      127     5970 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/error.rs
--rw-r--r--   0     1001      127     2519 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/input.rs
--rw-r--r--   0     1001      127     3242 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/internal.rs
--rw-r--r--   0     1001      127     1004 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/kind.rs
--rw-r--r--   0     1001      127     2685 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/mod.rs
--rw-r--r--   0     1001      127    17487 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/expression.rs
--rw-r--r--   0     1001      127     2212 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/gate.rs
--rw-r--r--   0     1001      127    40974 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/instruction.rs
--rw-r--r--   0     1001      127     1380 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/error.rs
--rw-r--r--   0     1001      127    17439 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/mod.rs
--rw-r--r--   0     1001      127     4222 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/quoted_strings.rs
--rw-r--r--   0     1001      127     3357 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs
--rw-r--r--   0     1001      127     4162 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/macros.rs
--rw-r--r--   0     1001      127     2446 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/mod.rs
--rw-r--r--   0     1001      127     5841 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/token.rs
--rw-r--r--   0     1001      127    25985 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/control_flow_graph.rs
--rw-r--r--   0     1001      127      974 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/mod.rs
--rw-r--r--   0     1001      127     9591 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/qubit_graph.rs
--rw-r--r--   0     1001      127      889 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
--rw-r--r--   0     1001      127     1329 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/test_programs.rs
--rw-r--r--   0     1001      127    23626 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/calibration.rs
--rw-r--r--   0     1001      127     7227 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/calibration_set.rs
--rw-r--r--   0     1001      127     2283 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/leftover.rs
--rw-r--r--   0     1001      127     3068 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/mod.rs
--rw-r--r--   0     1001      127     2252 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/result.rs
--rw-r--r--   0     1001      127     2725 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/syntax.rs
--rw-r--r--   0     1001      127     8742 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/frame.rs
--rw-r--r--   0     1001      127    17109 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/memory.rs
--rw-r--r--   0     1001      127    51116 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/mod.rs
--rw-r--r--   0     1001      127    26031 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/graph.rs
--rw-r--r--   0     1001      127    20046 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/graphviz_dot.rs
--rw-r--r--   0     1001      127      456 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/mod.rs
--rw-r--r--   0     1001      127    16670 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/schedule.rs
--rw-r--r--   0     1001      127     2678 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
--rw-r--r--   0     1001      127     1560 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
--rw-r--r--   0     1001      127     1166 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
--rw-r--r--   0     1001      127     1732 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
--rw-r--r--   0     1001      127     1112 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
--rw-r--r--   0     1001      127     1195 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
--rw-r--r--   0     1001      127     1780 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
--rw-r--r--   0     1001      127     1653 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
--rw-r--r--   0     1001      127     1003 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
--rw-r--r--   0     1001      127     1032 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
--rw-r--r--   0     1001      127      552 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
--rw-r--r--   0     1001      127     1540 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
--rw-r--r--   0     1001      127     1073 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
--rw-r--r--   0     1001      127     1338 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
--rw-r--r--   0     1001      127     1866 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
--rw-r--r--   0     1001      127      854 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
--rw-r--r--   0     1001      127      867 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
--rw-r--r--   0     1001      127      887 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
--rw-r--r--   0     1001      127     1892 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
--rw-r--r--   0     1001      127      839 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
--rw-r--r--   0     1001      127      768 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
--rw-r--r--   0     1001      127      591 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
--rw-r--r--   0     1001      127      793 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
--rw-r--r--   0     1001      127      852 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
--rw-r--r--   0     1001      127      585 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
--rw-r--r--   0     1001      127      227 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
--rw-r--r--   0     1001      127      136 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
--rw-r--r--   0     1001      127      215 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
--rw-r--r--   0     1001      127      476 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
--rw-r--r--   0     1001      127      210 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
--rw-r--r--   0     1001      127      141 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
--rw-r--r--   0     1001      127      159 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
--rw-r--r--   0     1001      127      309 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
--rw-r--r--   0     1001      127      261 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
--rw-r--r--   0     1001      127      155 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
--rw-r--r--   0     1001      127      254 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
--rw-r--r--   0     1001      127      174 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
--rw-r--r--   0     1001      127      167 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
--rw-r--r--   0     1001      127     3755 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
--rw-r--r--   0     1001      127      425 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
--rw-r--r--   0     1001      127    35001 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/type_check.rs
--rw-r--r--   0     1001      127     2422 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/quil.rs
--rw-r--r--   0     1001      127     2749 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/reserved.rs
--rw-r--r--   0     1001      127     2109 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/validation/identifier.rs
--rw-r--r--   0     1001      127       20 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/validation/mod.rs
--rw-r--r--   0     1001      127      724 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/calibration_test.rs
--rw-r--r--   0     1001      127      742 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz.quil
--rw-r--r--   0     1001      127     1888 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz_phase.quil
--rw-r--r--   0     1001      127     3266 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_measure.quil
--rw-r--r--   0     1001      127     1588 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_rx.quil
--rw-r--r--   0     1001      127     1786 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_xy.quil
--rw-r--r--   0     1001      127      747 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
--rw-r--r--   0     1001      127     1797 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
--rw-r--r--   0     1001      127     3187 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
--rw-r--r--   0     1001      127     1519 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
--rw-r--r--   0     1001      127     1719 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 quil-0.9.0rc0/quil-py/Cargo.toml
--rw-r--r--   0     1001      127      203 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/.flake8
--rw-r--r--   0     1001      127       10 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/.stubtest-allowlist
--rw-r--r--   0     1001      127    20540 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/CHANGELOG.md
--rw-r--r--   0     1001      127      858 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/Makefile.toml
--rw-r--r--   0     1001      127      777 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/README-py.md
--rw-r--r--   0     1001      127      337 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/README.md
--rw-r--r--   0     1001      127       71 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/build.rs
--rw-r--r--   0     1001      127      404 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/make_docs.py
--rw-r--r--   0     1001      127      135 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/index.html
--rw-r--r--   0     1001      127    34673 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/quil/quil.html
--rw-r--r--   0     1001      127    34581 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/quil.html
--rw-r--r--   0     1001      127    20706 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/search.js
--rw-r--r--   0     1001      127    36038 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/poetry.lock
--rw-r--r--   0     1001      127      283 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/__init__.pyi
--rw-r--r--   0     1001      127       30 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7690 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127      124 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91321 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127      129 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/program/__init__.py
--rw-r--r--   0     1001      127    18326 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/program/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/py.typed
--rw-r--r--   0     1001      127      161 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/__init__.py
--rw-r--r--   0     1001      127       39 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127       41 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/identifier.py
--rw-r--r--   0     1001      127      439 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127    34593 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil.html
--rw-r--r--   0     1001      127     6656 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/expression.rs
--rw-r--r--   0     1001      127     2838 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     1251 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/circuit.rs
--rw-r--r--   0     1001      127    11440 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/classical.rs
--rw-r--r--   0     1001      127     4295 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     5561 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9507 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/frame.rs
--rw-r--r--   0     1001      127     8394 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/gate.rs
--rw-r--r--   0     1001      127     1056 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/measurement.rs
--rw-r--r--   0     1001      127     8741 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1852 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/pragma.rs
--rw-r--r--   0     1001      127      978 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      738 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/reset.rs
--rw-r--r--   0     1001      127     1591 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/timing.rs
--rw-r--r--   0     1001      127     2443 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1967 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/lib.rs
--rw-r--r--   0     1001      127     2701 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/analysis.rs
--rw-r--r--   0     1001      127     4156 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/calibration.rs
--rw-r--r--   0     1001      127     2774 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/frame.rs
--rw-r--r--   0     1001      127      897 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/memory.rs
--rw-r--r--   0     1001      127    12676 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/mod.rs
--rw-r--r--   0     1001      127     1696 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/scheduling.rs
--rw-r--r--   0     1001      127     1136 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/validation/identifier.rs
--rw-r--r--   0     1001      127      151 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/validation/mod.rs
--rw-r--r--   0     1001      127     1665 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/instructions/test_copy.py
--rw-r--r--   0     1001      127      351 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/instructions/test_gate.py
--rw-r--r--   0     1001      127      137 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/program/__snapshots__/test_program.ambr
--rw-r--r--   0     1001      127     4566 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/program/test_program.py
--rw-r--r--   0     1001      127     1023 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/test_eq.py
--rw-r--r--   0     1001      127    50481 2024-04-16 22:48:12.000000 quil-0.9.0rc0/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 quil-0.9.0rc0/Cargo.toml
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 quil-0.9.0rc0/pyproject.toml
--rw-r--r--   0     1001      127      129 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/program/__init__.py
--rw-r--r--   0     1001      127    18326 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/program/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/py.typed
--rw-r--r--   0     1001      127      124 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91321 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127       30 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7690 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127      283 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/__init__.pyi
--rw-r--r--   0     1001      127       41 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/identifier.py
--rw-r--r--   0     1001      127      161 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/__init__.py
--rw-r--r--   0     1001      127       39 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127      439 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127      777 2024-04-16 22:48:07.000000 quil-0.9.0rc0/README-py.md
--rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 quil-0.9.0rc0/PKG-INFO
+-rw-r--r--   0     1001      127     1419 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/Cargo.toml
+-rw-r--r--   0     1001      127    44400 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/CHANGELOG.md
+-rw-r--r--   0     1001      127      954 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/README.md
+-rw-r--r--   0     1001      127     1692 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/corpus.rs
+-rw-r--r--   0     1001      127      941 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/get_frames_for_instruction.rs
+-rw-r--r--   0     1001      127      985 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/parser.rs
+-rw-r--r--   0     1001      127   803952 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/sample-calibrations.quil
+-rw-r--r--   0     1001      127     1478 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/scheduled_program_from_program.rs
+-rw-r--r--   0     1001      127      969 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/simplification.rs
+-rw-r--r--   0     1001      127    12979 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/benches/test_expressions.txt
+-rw-r--r--   0     1001      127     6316 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/examples/generate_test_expressions.rs
+-rw-r--r--   0     1001      127    38082 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/expression/mod.rs
+-rw-r--r--   0     1001      127    34338 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/expression/simplification/by_hand.rs
+-rw-r--r--   0     1001      127    12745 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/expression/simplification/mod.rs
+-rw-r--r--   0     1001      127     1002 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/hash.rs
+-rw-r--r--   0     1001      127     5302 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     6478 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127     9937 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     5260 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     6939 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9842 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/frame.rs
+-rw-r--r--   0     1001      127    43954 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/gate.rs
+-rw-r--r--   0     1001      127      771 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127    39443 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1798 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127     3425 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      654 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/reset.rs
+-rw-r--r--   0     1001      127      133 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
+-rw-r--r--   0     1001      127      133 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
+-rw-r--r--   0     1001      127      124 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
+-rw-r--r--   0     1001      127      167 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
+-rw-r--r--   0     1001      127      160 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
+-rw-r--r--   0     1001      127      109 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
+-rw-r--r--   0     1001      127      141 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
+-rw-r--r--   0     1001      127      125 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
+-rw-r--r--   0     1001      127      191 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
+-rw-r--r--   0     1001      127      178 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
+-rw-r--r--   0     1001      127      139 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
+-rw-r--r--   0     1001      127      143 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
+-rw-r--r--   0     1001      127     1528 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     3666 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1910 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/lib.rs
+-rw-r--r--   0     1001      127     1013 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/macros.rs
+-rw-r--r--   0     1001      127    36217 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/command.rs
+-rw-r--r--   0     1001      127    23080 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/common.rs
+-rw-r--r--   0     1001      127     5970 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/error.rs
+-rw-r--r--   0     1001      127     2519 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/input.rs
+-rw-r--r--   0     1001      127     3242 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/internal.rs
+-rw-r--r--   0     1001      127     1004 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/kind.rs
+-rw-r--r--   0     1001      127     2685 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/error/mod.rs
+-rw-r--r--   0     1001      127    17487 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/expression.rs
+-rw-r--r--   0     1001      127     2212 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/gate.rs
+-rw-r--r--   0     1001      127    40974 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/instruction.rs
+-rw-r--r--   0     1001      127     1380 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/error.rs
+-rw-r--r--   0     1001      127    17439 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/mod.rs
+-rw-r--r--   0     1001      127     4222 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/quoted_strings.rs
+-rw-r--r--   0     1001      127     3357 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs
+-rw-r--r--   0     1001      127     4162 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/macros.rs
+-rw-r--r--   0     1001      127     2446 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/mod.rs
+-rw-r--r--   0     1001      127     5841 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/parser/token.rs
+-rw-r--r--   0     1001      127    25985 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/control_flow_graph.rs
+-rw-r--r--   0     1001      127      974 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/mod.rs
+-rw-r--r--   0     1001      127     9591 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/qubit_graph.rs
+-rw-r--r--   0     1001      127      889 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
+-rw-r--r--   0     1001      127     1329 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/analysis/test_programs.rs
+-rw-r--r--   0     1001      127    23626 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/calibration.rs
+-rw-r--r--   0     1001      127     7227 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/calibration_set.rs
+-rw-r--r--   0     1001      127     2283 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/leftover.rs
+-rw-r--r--   0     1001      127     3068 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/mod.rs
+-rw-r--r--   0     1001      127     2252 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/result.rs
+-rw-r--r--   0     1001      127     2725 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/error/syntax.rs
+-rw-r--r--   0     1001      127     8742 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/frame.rs
+-rw-r--r--   0     1001      127    17109 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/memory.rs
+-rw-r--r--   0     1001      127    51116 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/mod.rs
+-rw-r--r--   0     1001      127    26031 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/graph.rs
+-rw-r--r--   0     1001      127    20046 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/graphviz_dot.rs
+-rw-r--r--   0     1001      127      456 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/mod.rs
+-rw-r--r--   0     1001      127    16670 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/schedule.rs
+-rw-r--r--   0     1001      127     2678 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
+-rw-r--r--   0     1001      127     1560 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
+-rw-r--r--   0     1001      127     1166 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
+-rw-r--r--   0     1001      127     1732 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
+-rw-r--r--   0     1001      127     1112 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
+-rw-r--r--   0     1001      127     1195 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
+-rw-r--r--   0     1001      127     1780 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
+-rw-r--r--   0     1001      127     1653 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
+-rw-r--r--   0     1001      127     1003 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
+-rw-r--r--   0     1001      127     1032 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
+-rw-r--r--   0     1001      127      552 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
+-rw-r--r--   0     1001      127     1540 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
+-rw-r--r--   0     1001      127     1073 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
+-rw-r--r--   0     1001      127     1338 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
+-rw-r--r--   0     1001      127     1866 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
+-rw-r--r--   0     1001      127      854 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
+-rw-r--r--   0     1001      127      867 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
+-rw-r--r--   0     1001      127      887 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
+-rw-r--r--   0     1001      127     1892 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
+-rw-r--r--   0     1001      127      839 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
+-rw-r--r--   0     1001      127      768 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
+-rw-r--r--   0     1001      127      591 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
+-rw-r--r--   0     1001      127      793 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
+-rw-r--r--   0     1001      127      852 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
+-rw-r--r--   0     1001      127      585 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
+-rw-r--r--   0     1001      127      227 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
+-rw-r--r--   0     1001      127      136 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
+-rw-r--r--   0     1001      127      215 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
+-rw-r--r--   0     1001      127      476 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
+-rw-r--r--   0     1001      127      210 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
+-rw-r--r--   0     1001      127      141 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
+-rw-r--r--   0     1001      127      159 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
+-rw-r--r--   0     1001      127      309 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
+-rw-r--r--   0     1001      127      261 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
+-rw-r--r--   0     1001      127      155 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
+-rw-r--r--   0     1001      127      254 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
+-rw-r--r--   0     1001      127      174 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
+-rw-r--r--   0     1001      127      167 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
+-rw-r--r--   0     1001      127     3755 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
+-rw-r--r--   0     1001      127      425 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
+-rw-r--r--   0     1001      127    35001 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/program/type_check.rs
+-rw-r--r--   0     1001      127     2422 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/quil.rs
+-rw-r--r--   0     1001      127     2749 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/reserved.rs
+-rw-r--r--   0     1001      127     2109 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/validation/identifier.rs
+-rw-r--r--   0     1001      127       20 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/src/validation/mod.rs
+-rw-r--r--   0     1001      127      724 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/calibration_test.rs
+-rw-r--r--   0     1001      127      742 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz.quil
+-rw-r--r--   0     1001      127     1888 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz_phase.quil
+-rw-r--r--   0     1001      127     3266 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_measure.quil
+-rw-r--r--   0     1001      127     1588 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_rx.quil
+-rw-r--r--   0     1001      127     1786 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/programs/calibration_xy.quil
+-rw-r--r--   0     1001      127      747 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
+-rw-r--r--   0     1001      127     1797 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
+-rw-r--r--   0     1001      127     3187 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
+-rw-r--r--   0     1001      127     1519 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
+-rw-r--r--   0     1001      127     1719 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 quil-0.9.1rc0/quil-py/Cargo.toml
+-rw-r--r--   0     1001      127      203 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/.flake8
+-rw-r--r--   0     1001      127       10 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/.stubtest-allowlist
+-rw-r--r--   0     1001      127    20835 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/CHANGELOG.md
+-rw-r--r--   0     1001      127     1258 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/Makefile.toml
+-rw-r--r--   0     1001      127      777 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/README-py.md
+-rw-r--r--   0     1001      127      337 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/README.md
+-rw-r--r--   0     1001      127       71 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/build.rs
+-rw-r--r--   0     1001      127      403 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/make_docs.py
+-rw-r--r--   0     1001      127      135 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/index.html
+-rw-r--r--   0     1001      127    34673 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/quil/quil.html
+-rw-r--r--   0     1001      127    34581 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/quil.html
+-rw-r--r--   0     1001      127    20706 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/out/search.js
+-rw-r--r--   0     1001      127    32817 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/poetry.lock
+-rw-r--r--   0     1001      127      283 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/__init__.pyi
+-rw-r--r--   0     1001      127       30 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7528 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127      123 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91194 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127      127 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/program/__init__.py
+-rw-r--r--   0     1001      127    17967 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/py.typed
+-rw-r--r--   0     1001      127      160 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       39 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127       41 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/identifier.py
+-rw-r--r--   0     1001      127      419 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127    34593 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/quil.html
+-rw-r--r--   0     1001      127     6656 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/expression.rs
+-rw-r--r--   0     1001      127     2838 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     1251 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127    11440 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     4295 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     5561 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9507 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/frame.rs
+-rw-r--r--   0     1001      127     8394 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/gate.rs
+-rw-r--r--   0     1001      127     1056 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127     8741 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1852 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127      978 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      738 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/reset.rs
+-rw-r--r--   0     1001      127     1591 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     2443 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1967 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/lib.rs
+-rw-r--r--   0     1001      127     2982 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/analysis.rs
+-rw-r--r--   0     1001      127     4156 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/calibration.rs
+-rw-r--r--   0     1001      127     2774 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/frame.rs
+-rw-r--r--   0     1001      127      897 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/memory.rs
+-rw-r--r--   0     1001      127    12676 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/mod.rs
+-rw-r--r--   0     1001      127     1970 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/program/scheduling.rs
+-rw-r--r--   0     1001      127     1136 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/validation/identifier.rs
+-rw-r--r--   0     1001      127      151 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/src/validation/mod.rs
+-rw-r--r--   0     1001      127     1617 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/instructions/test_copy.py
+-rw-r--r--   0     1001      127      351 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/instructions/test_gate.py
+-rw-r--r--   0     1001      127      137 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/program/__snapshots__/test_program.ambr
+-rw-r--r--   0     1001      127     4596 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/program/test_program.py
+-rw-r--r--   0     1001      127     1025 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil-py/test/test_eq.py
+-rw-r--r--   0     1001      127    50481 2024-04-17 20:38:08.000000 quil-0.9.1rc0/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 quil-0.9.1rc0/Cargo.toml
+-rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 quil-0.9.1rc0/pyproject.toml
+-rw-r--r--   0     1001      127      127 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/program/__init__.py
+-rw-r--r--   0     1001      127    17967 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/py.typed
+-rw-r--r--   0     1001      127      123 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91194 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127       30 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7528 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127      283 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/__init__.pyi
+-rw-r--r--   0     1001      127       41 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/identifier.py
+-rw-r--r--   0     1001      127      160 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       39 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127      419 2024-04-17 20:38:00.000000 quil-0.9.1rc0/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127      777 2024-04-17 20:38:00.000000 quil-0.9.1rc0/README-py.md
+-rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 quil-0.9.1rc0/PKG-INFO
```

### Comparing `quil-0.9.0rc0/quil-rs/Cargo.toml` & `quil-0.9.1rc0/quil-rs/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "quil-rs"
 description = "Rust tooling for Quil (Quantum Instruction Language)"
-version = "0.25.0-rc.0"
+version = "0.25.1-rc.0"
 edition = "2021"
 rust-version = "1.70"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rust"
 keywords = ["Quil", "Quantum", "Rigetti"]
 categories = ["parser-implementations", "science", "compilers", "emulators"]
```

### Comparing `quil-0.9.0rc0/quil-rs/CHANGELOG.md` & `quil-0.9.1rc0/quil-rs/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## 0.25.1-rc.0
+
+### Features
+
+- Support constructing ControlFlowGraph and BasicBlocks. (#359)
+
+## 0.25.0
+
+### Breaking Changes
+
+- Program instruction iteration and serialization is deterministic. (#355)
+
+### Fixes
+
+- Program equality is sensitive to the order of calibration instructions. (#357)
+
 ## 0.25.0-rc.0
 
 ### Breaking Changes
 
 - Program instruction iteration and serialization is deterministic. (#355)
 
 ### Fixes
```

### Comparing `quil-0.9.0rc0/quil-rs/README.md` & `quil-0.9.1rc0/quil-rs/README.md`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/benches/corpus.rs` & `quil-0.9.1rc0/quil-rs/benches/corpus.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/benches/get_frames_for_instruction.rs` & `quil-0.9.1rc0/quil-rs/benches/get_frames_for_instruction.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/benches/parser.rs` & `quil-0.9.1rc0/quil-rs/benches/parser.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/benches/sample-calibrations.quil` & `quil-0.9.1rc0/quil-rs/benches/sample-calibrations.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/benches/scheduled_program_from_program.rs` & `quil-0.9.1rc0/quil-rs/benches/scheduled_program_from_program.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/benches/simplification.rs` & `quil-0.9.1rc0/quil-rs/benches/simplification.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/benches/test_expressions.txt` & `quil-0.9.1rc0/quil-rs/benches/test_expressions.txt`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/examples/generate_test_expressions.rs` & `quil-0.9.1rc0/quil-rs/examples/generate_test_expressions.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/expression/mod.rs` & `quil-0.9.1rc0/quil-rs/src/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/expression/simplification/by_hand.rs` & `quil-0.9.1rc0/quil-rs/src/expression/simplification/by_hand.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/expression/simplification/mod.rs` & `quil-0.9.1rc0/quil-rs/src/expression/simplification/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/hash.rs` & `quil-0.9.1rc0/quil-rs/src/hash.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/calibration.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/circuit.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/classical.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/control_flow.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/declaration.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/frame.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/gate.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/measurement.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/mod.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/pragma.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/qubit.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/reset.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/timing.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/instruction/waveform.rs` & `quil-0.9.1rc0/quil-rs/src/instruction/waveform.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/lib.rs` & `quil-0.9.1rc0/quil-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/macros.rs` & `quil-0.9.1rc0/quil-rs/src/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/command.rs` & `quil-0.9.1rc0/quil-rs/src/parser/command.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/common.rs` & `quil-0.9.1rc0/quil-rs/src/parser/common.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/error/error.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/error/input.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/input.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/error/internal.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/internal.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/error/kind.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/kind.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/error/mod.rs` & `quil-0.9.1rc0/quil-rs/src/parser/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/expression.rs` & `quil-0.9.1rc0/quil-rs/src/parser/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/gate.rs` & `quil-0.9.1rc0/quil-rs/src/parser/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/instruction.rs` & `quil-0.9.1rc0/quil-rs/src/parser/instruction.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/lexer/error.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/lexer/mod.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/lexer/quoted_strings.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/quoted_strings.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs` & `quil-0.9.1rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/macros.rs` & `quil-0.9.1rc0/quil-rs/src/parser/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/mod.rs` & `quil-0.9.1rc0/quil-rs/src/parser/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/parser/token.rs` & `quil-0.9.1rc0/quil-rs/src/parser/token.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/analysis/control_flow_graph.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/control_flow_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/analysis/mod.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/analysis/qubit_graph.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/qubit_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap` & `quil-0.9.1rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/analysis/test_programs.rs` & `quil-0.9.1rc0/quil-rs/src/program/analysis/test_programs.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/calibration.rs` & `quil-0.9.1rc0/quil-rs/src/program/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/calibration_set.rs` & `quil-0.9.1rc0/quil-rs/src/program/calibration_set.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/error/leftover.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/leftover.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/error/mod.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/error/result.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/result.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/error/syntax.rs` & `quil-0.9.1rc0/quil-rs/src/program/error/syntax.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/frame.rs` & `quil-0.9.1rc0/quil-rs/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/memory.rs` & `quil-0.9.1rc0/quil-rs/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/mod.rs` & `quil-0.9.1rc0/quil-rs/src/program/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/graph.rs` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/graphviz_dot.rs` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/graphviz_dot.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/schedule.rs` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/schedule.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap` & `quil-0.9.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap` & `quil-0.9.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/program/type_check.rs` & `quil-0.9.1rc0/quil-rs/src/program/type_check.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/quil.rs` & `quil-0.9.1rc0/quil-rs/src/quil.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/reserved.rs` & `quil-0.9.1rc0/quil-rs/src/reserved.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/src/validation/identifier.rs` & `quil-0.9.1rc0/quil-rs/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/calibration_test.rs` & `quil-0.9.1rc0/quil-rs/tests/calibration_test.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz_phase.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_cz_phase.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/programs/calibration_measure.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_measure.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/programs/calibration_rx.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_rx.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/programs/calibration_xy.quil` & `quil-0.9.1rc0/quil-rs/tests/programs/calibration_xy.quil`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap` & `quil-0.9.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/Cargo.toml` & `quil-0.9.1rc0/quil-py/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "quil-py"
 description = "Python bindings for quil-rs"
-version = "0.9.0-rc.0"
+version = "0.9.1-rc.0"
 edition = "2021"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rs"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "parsers", "science", "emulators"]
 readme = "./README.md"
 
@@ -18,15 +18,15 @@
 #
 # Downstream Rust code (including code in `bin/`, `examples/`, and `tests/`) will not be able
 # to `use quil;` unless the "lib" and "rlib" crate type is also included:
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
 ndarray.workspace = true
-quil-rs = { path = "../quil-rs", version = "0.25.0-rc.0" }
+quil-rs = { path = "../quil-rs", version = "0.25.1-rc.0" }
 strum.workspace = true
 # pyo3 dependencies should be updated together
 numpy = "0.20.0"
 pyo3 = { version = "0.20.3", features = ["indexmap"] }
 rigetti-pyo3 = {version = "0.3.4", features = ["indexmap"]}
 indexmap.workspace = true
```

### Comparing `quil-0.9.0rc0/quil-py/CHANGELOG.md` & `quil-0.9.1rc0/quil-py/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## 0.9.1-rc.0
+
+### Features
+
+- Support constructing ControlFlowGraph and BasicBlocks. (#359)
+
+## 0.9.0
+
+### Breaking Changes
+
+- Program instruction iteration and serialization is deterministic. (#355)
+
+### Fixes
+
+- Program equality is sensitive to the order of calibration instructions. (#357)
+
 ## 0.9.0-rc.0
 
 ### Breaking Changes
 
 - Program instruction iteration and serialization is deterministic. (#355)
 
 ### Fixes
```

### Comparing `quil-0.9.0rc0/quil-py/Makefile.toml` & `quil-0.9.1rc0/quil-py/Makefile.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,40 @@
 args = ["install"]
 
 [tasks.install-quil]
 command = "poetry"
 args = ["run", "maturin", "develop"]
 
 [tasks.stubtest]
+dependencies = ["poetry-install"]
 command = "poetry"
 args = ["run", "stubtest", "--allowlist", ".stubtest-allowlist", "quil"]
 
 [tasks.stubtest-flow]
 dependencies = [
     "poetry-install",
     "install-quil",
     "stubtest",
 ]
 
+[tasks.format]
+dependencies = ["poetry-install"]
+command = "poetry"
+args = ["run", "ruff", "format"]
+
+[tasks.check-format]
+dependencies = ["poetry-install"]
+command = "poetry"
+args = ["run", "ruff", "format", "--check"]
+
+[tasks.lint]
+dependencies = ["poetry-install"]
+command = "poetry"
+args = ["run", "ruff", "check"]
+
 [tasks.pytest]
 command = "poetry"
 args = ["run", "pytest"]
 
 [tasks.pytest-flow]
 dependencies = [
     "poetry-install",
@@ -33,11 +49,17 @@
 
 [tasks.docs]
 dependencies = ["poetry-install", "install-quil"]
 command = "poetry"
 args = ["run", "pdoc", "-o", "build/docs", "quil", "!quil.quil", "--logo", "https://qcs.rigetti.com/static/img/rigetti-logo.svg"]
 
 [tasks.dev-flow]
-dependencies = ["dev-test-flow", "pytest-flow", "stubtest"]
+dependencies = [
+    "dev-test-flow",
+    "pytest-flow",
+    "stubtest",
+    "lint",
+    "check-format"
+]
 
 [tasks.default]
 alias = "dev-flow"
```

### Comparing `quil-0.9.0rc0/quil-py/README-py.md` & `quil-0.9.1rc0/quil-py/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/out/quil/quil.html` & `quil-0.9.1rc0/quil-py/out/quil/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/out/quil.html` & `quil-0.9.1rc0/quil-py/out/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/out/search.js` & `quil-0.9.1rc0/quil-py/out/search.js`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/poetry.lock` & `quil-0.9.1rc0/quil-py/poetry.lock`

 * *Files 13% similar despite different names*

```diff
@@ -30,77 +30,14 @@
 cov = ["attrs[tests]", "coverage-enable-subprocess", "coverage[toml] (>=5.3)"]
 dev = ["attrs[docs,tests]"]
 docs = ["furo", "myst-parser", "sphinx", "sphinx-notfound-page", "sphinxcontrib-towncrier", "towncrier", "zope.interface"]
 tests = ["attrs[tests-no-zope]", "zope.interface"]
 tests-no-zope = ["cloudpickle", "cloudpickle", "hypothesis", "hypothesis", "mypy (>=0.971,<0.990)", "mypy (>=0.971,<0.990)", "pympler", "pympler", "pytest (>=4.3.0)", "pytest (>=4.3.0)", "pytest-mypy-plugins", "pytest-mypy-plugins", "pytest-xdist[psutil]", "pytest-xdist[psutil]"]
 
 [[package]]
-name = "black"
-version = "23.1.0"
-description = "The uncompromising code formatter."
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "black-23.1.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:b6a92a41ee34b883b359998f0c8e6eb8e99803aa8bf3123bf2b2e6fec505a221"},
-    {file = "black-23.1.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:57c18c5165c1dbe291d5306e53fb3988122890e57bd9b3dcb75f967f13411a26"},
-    {file = "black-23.1.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:9880d7d419bb7e709b37e28deb5e68a49227713b623c72b2b931028ea65f619b"},
-    {file = "black-23.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104"},
-    {file = "black-23.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:9afd3f493666a0cd8f8df9a0200c6359ac53940cbde049dcb1a7eb6ee2dd7074"},
-    {file = "black-23.1.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:bfffba28dc52a58f04492181392ee380e95262af14ee01d4bc7bb1b1c6ca8d27"},
-    {file = "black-23.1.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c1c476bc7b7d021321e7d93dc2cbd78ce103b84d5a4cf97ed535fbc0d6660648"},
-    {file = "black-23.1.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:382998821f58e5c8238d3166c492139573325287820963d2f7de4d518bd76958"},
-    {file = "black-23.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2bf649fda611c8550ca9d7592b69f0637218c2369b7744694c5e4902873b2f3a"},
-    {file = "black-23.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:121ca7f10b4a01fd99951234abdbd97728e1240be89fde18480ffac16503d481"},
-    {file = "black-23.1.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:a8471939da5e824b891b25751955be52ee7f8a30a916d570a5ba8e0f2eb2ecad"},
-    {file = "black-23.1.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8178318cb74f98bc571eef19068f6ab5613b3e59d4f47771582f04e175570ed8"},
-    {file = "black-23.1.0-cp37-cp37m-win_amd64.whl", hash = "sha256:a436e7881d33acaf2536c46a454bb964a50eff59b21b51c6ccf5a40601fbef24"},
-    {file = "black-23.1.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:a59db0a2094d2259c554676403fa2fac3473ccf1354c1c63eccf7ae65aac8ab6"},
-    {file = "black-23.1.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:0052dba51dec07ed029ed61b18183942043e00008ec65d5028814afaab9a22fd"},
-    {file = "black-23.1.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:49f7b39e30f326a34b5c9a4213213a6b221d7ae9d58ec70df1c4a307cf2a1580"},
-    {file = "black-23.1.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:162e37d49e93bd6eb6f1afc3e17a3d23a823042530c37c3c42eeeaf026f38468"},
-    {file = "black-23.1.0-cp38-cp38-win_amd64.whl", hash = "sha256:8b70eb40a78dfac24842458476135f9b99ab952dd3f2dab738c1881a9b38b753"},
-    {file = "black-23.1.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:a29650759a6a0944e7cca036674655c2f0f63806ddecc45ed40b7b8aa314b651"},
-    {file = "black-23.1.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:bb460c8561c8c1bec7824ecbc3ce085eb50005883a6203dcfb0122e95797ee06"},
-    {file = "black-23.1.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:c91dfc2c2a4e50df0026f88d2215e166616e0c80e86004d0003ece0488db2739"},
-    {file = "black-23.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2a951cc83ab535d248c89f300eccbd625e80ab880fbcfb5ac8afb5f01a258ac9"},
-    {file = "black-23.1.0-cp39-cp39-win_amd64.whl", hash = "sha256:0680d4380db3719ebcfb2613f34e86c8e6d15ffeabcf8ec59355c5e7b85bb555"},
-    {file = "black-23.1.0-py3-none-any.whl", hash = "sha256:7a0f701d314cfa0896b9001df70a530eb2472babb76086344e688829efd97d32"},
-    {file = "black-23.1.0.tar.gz", hash = "sha256:b0bd97bea8903f5a2ba7219257a44e3f1f9d00073d6cc1add68f0beec69692ac"},
-]
-
-[package.dependencies]
-click = ">=8.0.0"
-mypy-extensions = ">=0.4.3"
-packaging = ">=22.0"
-pathspec = ">=0.9.0"
-platformdirs = ">=2"
-tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
-typing-extensions = {version = ">=3.10.0.0", markers = "python_version < \"3.10\""}
-
-[package.extras]
-colorama = ["colorama (>=0.4.3)"]
-d = ["aiohttp (>=3.7.4)"]
-jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
-uvloop = ["uvloop (>=0.15.2)"]
-
-[[package]]
-name = "click"
-version = "8.1.3"
-description = "Composable command line interface toolkit"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
-    {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
-]
-
-[package.dependencies]
-colorama = {version = "*", markers = "platform_system == \"Windows\""}
-
-[[package]]
 name = "colorama"
 version = "0.4.6"
 description = "Cross-platform colored terminal text."
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
@@ -359,25 +296,14 @@
 python-versions = ">=3.7"
 files = [
     {file = "packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
     {file = "packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
 ]
 
 [[package]]
-name = "pathspec"
-version = "0.11.0"
-description = "Utility library for gitignore style pattern matching of file paths."
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "pathspec-0.11.0-py3-none-any.whl", hash = "sha256:3a66eb970cbac598f9e5ccb5b2cf58930cd8e3ed86d393d541eaf2d8b1705229"},
-    {file = "pathspec-0.11.0.tar.gz", hash = "sha256:64d338d4e0914e91c1792321e6907b5a593f1ab1851de7fc269557a21b30ebbc"},
-]
-
-[[package]]
 name = "pdoc"
 version = "14.1.0"
 description = "API Documentation for Python Projects"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "pdoc-14.1.0-py3-none-any.whl", hash = "sha256:e8869dffe21296b3bd5545b28e7f07cae0656082aca43f8915323187e541b126"},
@@ -390,29 +316,14 @@
 MarkupSafe = "*"
 pygments = ">=2.12.0"
 
 [package.extras]
 dev = ["black", "hypothesis", "mypy", "pygments (>=2.14.0)", "pytest", "pytest-cov", "pytest-timeout", "ruff", "tox", "types-pygments"]
 
 [[package]]
-name = "platformdirs"
-version = "3.1.1"
-description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "platformdirs-3.1.1-py3-none-any.whl", hash = "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"},
-    {file = "platformdirs-3.1.1.tar.gz", hash = "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa"},
-]
-
-[package.extras]
-docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2.1)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
-
-[[package]]
 name = "pluggy"
 version = "1.0.0"
 description = "plugin and hook calling mechanisms for python"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
@@ -457,14 +368,40 @@
 pluggy = ">=0.12,<2.0"
 tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
 testing = ["argcomplete", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "xmlschema"]
 
 [[package]]
+name = "ruff"
+version = "0.3.7"
+description = "An extremely fast Python linter and code formatter, written in Rust."
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "ruff-0.3.7-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:0e8377cccb2f07abd25e84fc5b2cbe48eeb0fea9f1719cad7caedb061d70e5ce"},
+    {file = "ruff-0.3.7-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:15a4d1cc1e64e556fa0d67bfd388fed416b7f3b26d5d1c3e7d192c897e39ba4b"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d28bdf3d7dc71dd46929fafeec98ba89b7c3550c3f0978e36389b5631b793663"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:379b67d4f49774ba679593b232dcd90d9e10f04d96e3c8ce4a28037ae473f7bb"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c060aea8ad5ef21cdfbbe05475ab5104ce7827b639a78dd55383a6e9895b7c51"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:ebf8f615dde968272d70502c083ebf963b6781aacd3079081e03b32adfe4d58a"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d48098bd8f5c38897b03604f5428901b65e3c97d40b3952e38637b5404b739a2"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:da8a4fda219bf9024692b1bc68c9cff4b80507879ada8769dc7e985755d662ea"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c44e0149f1d8b48c4d5c33d88c677a4aa22fd09b1683d6a7ff55b816b5d074f"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:3050ec0af72b709a62ecc2aca941b9cd479a7bf2b36cc4562f0033d688e44fa1"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:a29cc38e4c1ab00da18a3f6777f8b50099d73326981bb7d182e54a9a21bb4ff7"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_i686.whl", hash = "sha256:5b15cc59c19edca917f51b1956637db47e200b0fc5e6e1878233d3a938384b0b"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:e491045781b1e38b72c91247cf4634f040f8d0cb3e6d3d64d38dcf43616650b4"},
+    {file = "ruff-0.3.7-py3-none-win32.whl", hash = "sha256:bc931de87593d64fad3a22e201e55ad76271f1d5bfc44e1a1887edd0903c7d9f"},
+    {file = "ruff-0.3.7-py3-none-win_amd64.whl", hash = "sha256:5ef0e501e1e39f35e03c2acb1d1238c595b8bb36cf7a170e7c1df1b73da00e74"},
+    {file = "ruff-0.3.7-py3-none-win_arm64.whl", hash = "sha256:789e144f6dc7019d1f92a812891c645274ed08af6037d11fc65fcbc183b7d59f"},
+    {file = "ruff-0.3.7.tar.gz", hash = "sha256:d5c1aebee5162c2226784800ae031f660c350e7a3402c4d1f8ea4e97e232e3ba"},
+]
+
+[[package]]
 name = "six"
 version = "1.16.0"
 description = "Python 2 and 3 compatibility utilities"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
@@ -521,8 +458,8 @@
 
 [package.extras]
 test = ["pytest (>=6.0.0)", "setuptools (>=65)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.8"
-content-hash = "0a3b0fa6670ec3156719cb56a052cce8f8fe11169745f976da20549182936840"
+content-hash = "c4cf08c102dd7ec09c483f00c9dbbabdca03917d1393809aafa65beab8253376"
```

### Comparing `quil-0.9.0rc0/quil-py/quil/expression/__init__.pyi` & `quil-0.9.1rc0/quil-py/quil/expression/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""
-The ``expression`` module contains classes for representing Quil expressions.
-"""
+"""The ``expression`` module contains classes for representing Quil expressions."""
+
 from enum import Enum
-from typing import Dict, final, Sequence, Optional, Union
+from typing import Dict, Optional, Sequence, Union, final
 
 from quil.instructions import MemoryReference
 
 class EvaluationError(ValueError):
-    """Error that may occur while evaluation an ``Expression``"""
+    """Error that may occur while evaluation an ``Expression``."""
 
 class ParseExpressionError(ValueError):
-    """Error that may occur while parsing an ``Expression``"""
+    """Error that may occur while parsing an ``Expression``."""
 
 @final
 class Expression:
-    """
-    A Quil expression.
+    """A Quil expression.
 
     # Variants:
     - ``address``: An address defined by a `quil.instructions.MemoryReference`.
     - ``function_call``: A `FunctionCallExpression`.
     - ``infix``: An `InfixExpression`.
     - ``number``: A number defined as a `complex`.
     - ``pi``: The constant ``pi``. No inner data.
@@ -41,24 +39,29 @@
 
     If the variant doesn't have inner data (e.g. ``pi``)
     - ``new_*``: Creates a new ``Expression`` for the variant
     """
 
     def inner(
         self,
-    ) -> Union[MemoryReference, FunctionCallExpression, InfixExpression, int, PrefixExpression, str,]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+    ) -> Union[
+        MemoryReference,
+        FunctionCallExpression,
+        InfixExpression,
+        int,
+        PrefixExpression,
+        str,
+    ]:
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     @staticmethod
     def parse(input: str) -> Expression:
-        """
-        Parses an ``Expression`` from a string. Raises a ``ParseExpressionError`` if the string
-        isn't a valid Quil expression.
+        """Parses an ``Expression`` from a string.
+
+        Raises a ``ParseExpressionError`` if the string isn't a valid Quil expression.
         """
     def is_address(self) -> bool: ...
     def is_function_call(self) -> bool: ...
     def is_infix(self) -> bool: ...
     def is_number(self) -> bool: ...
     def is_pi(self) -> bool: ...
     def is_prefix(self) -> bool: ...
@@ -86,79 +89,62 @@
     def as_number(self) -> Optional[complex]: ...
     def to_number(self) -> complex: ...
     def as_prefix(self) -> Optional[PrefixExpression]: ...
     def to_prefix(self) -> PrefixExpression: ...
     def as_variable(self) -> Optional[str]: ...
     def to_variable(self) -> str: ...
     def simplify(self):
-        """
-        Simplify the expression as much as possible, in-place.
-        """
+        """Simplify the expression as much as possible, in-place."""
         ...
     def into_simplified(self) -> "Expression":
-        """
-        Return a simplified copy of the expression.
-        """
+        """Return a simplified copy of the expression."""
     def evaluate(
         self,
         variables: Dict[str, complex],
         memory_references: Dict[str, Sequence[float]],
     ) -> complex:
-        """
-        Evaluate an expression, expecting that it may be fully reduced to a single complex number.
+        """Evaluate an expression, expecting that it may be fully reduced to a single complex number.
+
         If it cannot be reduced to a complex number, raises an ``EvaluationError``.
         """
         ...
     def substitute_variables(self, variable_values: Dict[str, "Expression"]) -> "Expression":
-        """
-        Returns a copy of the expression where every matching variable in `variable_values` is
-        replaced by the corresponding expression.
-        """
+        """Returns a copy of the expression where every matching variable in `variable_values` is replaced by the corresponding expression."""
         ...
     def to_real(self) -> float:
-        """
-        If this is a number with imaginary part "equal to" zero (of <em>small</em> absolute value), return
-        that number. Otherwise, raises an ``EvaluationError``
-        """
+        """If this is a number with imaginary part "equal to" zero (of <em>small</em> absolute value), return that number. Otherwise, raises an ``EvaluationError``."""
     def __add__(self, other: "Expression") -> "Expression": ...
     def __sub__(self, other: "Expression") -> "Expression": ...
     def __mul__(self, other: "Expression") -> "Expression": ...
     def __truediv__(self, other: "Expression") -> "Expression": ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
+        """Attempt to convert the instruction to a valid Quil string. Raises an exception if the instruction can't be converted to valid Quil."""
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format
-        that isn't valid Quil.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug
+        format that isn't valid Quil.
         """
 
 class FunctionCallExpression:
-    """
-    A Quil function call.
-    """
+    """A Quil function call."""
     @staticmethod
     def __new__(cls, function: ExpressionFunction, expression: Expression) -> "FunctionCallExpression": ...
     @property
     def function(self) -> ExpressionFunction: ...
     @function.setter
     def function(self, function: ExpressionFunction): ...
     @property
     def expression(self) -> Expression: ...
     @expression.setter
     def expression(self, expression: Expression): ...
 
 class InfixExpression:
-    """
-    A Quil infix expression.
-    """
+    """A Quil infix expression."""
     @staticmethod
     def __new__(cls, left: Expression, operator: InfixOperator, right: Expression): ...
     @property
     def left(self) -> Expression: ...
     @left.setter
     def left(self, expression: Expression): ...
     @property
@@ -167,50 +153,45 @@
     def operator(self, operator: InfixOperator): ...
     @property
     def right(self) -> Expression: ...
     @right.setter
     def right(self, expression: Expression): ...
 
 class PrefixExpression:
-    """
-    A Quil prefix expression.
-    """
+    """A Quil prefix expression."""
     @staticmethod
     def __new__(cls, operator: PrefixOperator, expression: Expression): ...
     @property
     def operator(self) -> PrefixOperator: ...
     @operator.setter
     def operator(self, operator: PrefixOperator): ...
     @property
     def expression(self) -> Expression: ...
     @expression.setter
     def expression(self, expression: Expression): ...
 
 @final
 class ExpressionFunction(Enum):
-    """
-    An enum representing a Quil function that can be applied to an expression.
-    """
+    """An enum representing a Quil function that can be applied to an expression."""
+
     Cis = "CIS"
     Cosine = "COSINE"
     Exponent = "EXPONENT"
     Sine = "SINE"
     SquareRoot = "SQUAREROOT"
 
 @final
 class PrefixOperator(Enum):
-    """
-    An enum that represents the operators supported on a prefix expression.
-    """
+    """An enum that represents the operators supported on a prefix expression."""
+
     Plus = "PLUS"
     Minus = "MINUS"
 
 @final
 class InfixOperator(Enum):
-    """
-    An enum that represents the operators supported on an infix expression.
-    """
+    """An enum that represents the operators supported on an infix expression."""
+
     Caret = "CARET"
     Plus = "PLUS"
     Minus = "MINUS"
     Slash = "SLASH"
     Star = "STAR"
```

### Comparing `quil-0.9.0rc0/quil-py/quil/instructions/__init__.pyi` & `quil-0.9.1rc0/quil-py/quil/instructions/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from enum import Enum
+from typing import Dict, List, Optional, Sequence, Tuple, Union, final
+
 import numpy as np
 from numpy.typing import NDArray
-from typing import Dict, List, Optional, Sequence, Tuple, Union, final
 from typing_extensions import Self
 
 from quil.expression import Expression
 
 @final
 class Instruction:
-    """
-    A Quil instruction. Each variant corresponds to a possible type of Quil instruction.
+    """A Quil instruction. Each variant corresponds to a possible type of Quil instruction.
 
     # Variants:
     - ``arithmetic``: An arithmetic expression defined by an ``Arithmetic``.
     - ``binary_logic``: A binary expression defined by a ``BinaryLogic``.
     - ``calibration_definition``: Corresponds to a `DEFCAL` instruction (not `DEFCAL MEASURE`)
     -     defined by a ``Calibration``.
     - ``capture``: Corresponds to a `CAPTURE` instruction
@@ -109,21 +109,17 @@
             ShiftPhase,
             Store,
             SwapPhases,
             UnaryLogic,
             WaveformDefinition,
         ],
     ) -> Self:
-        """
-        Returns a new ``Instruction`` from the given inner data.
-        """
+        """Returns a new ``Instruction`` from the given inner data."""
     def is_quil_t(self) -> bool:
-        """
-        Returns ``True`` if the instruction is a Quil-T instruction, ``False`` otherwise.
-        """
+        """Returns ``True`` if the instruction is a Quil-T instruction, ``False`` otherwise."""
         ...
     def inner(
         self,
     ) -> Union[
         Arithmetic,
         Calibration,
         Capture,
@@ -157,17 +153,15 @@
         ShiftFrequency,
         ShiftPhase,
         Store,
         SwapPhases,
         UnaryLogic,
         WaveformDefinition,
     ]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_arithmetic(self) -> bool: ...
     def is_binary_logic(self) -> bool: ...
     def is_calibration_definition(self) -> bool: ...
     def is_capture(self) -> bool: ...
     def is_circuit_definition(self) -> bool: ...
     def is_convert(self) -> bool: ...
@@ -201,99 +195,99 @@
     def is_shift_phase(self) -> bool: ...
     def is_unary_logic(self) -> bool: ...
     def is_store(self) -> bool: ...
     def is_swap_phases(self) -> bool: ...
     def is_waveform_definition(self) -> bool: ...
     def is_wait(self) -> bool: ...
     @staticmethod
-    def new_halt() -> "Instruction": ...
+    def new_halt() -> Instruction: ...
     @staticmethod
-    def new_nop() -> "Instruction": ...
+    def new_nop() -> Instruction: ...
     @staticmethod
-    def new_wait() -> "Instruction": ...
+    def new_wait() -> Instruction: ...
     @staticmethod
-    def from_arithmetic(inner: Arithmetic) -> "Instruction": ...
+    def from_arithmetic(inner: Arithmetic) -> Instruction: ...
     @staticmethod
-    def from_binary_logic(inner: BinaryLogic) -> "Instruction": ...
+    def from_binary_logic(inner: BinaryLogic) -> Instruction: ...
     @staticmethod
-    def from_calibration_definition(inner: Calibration) -> "Instruction": ...
+    def from_calibration_definition(inner: Calibration) -> Instruction: ...
     @staticmethod
-    def from_capture(inner: Capture) -> "Instruction": ...
+    def from_capture(inner: Capture) -> Instruction: ...
     @staticmethod
     def from_circuit_definition(
         inner: CircuitDefinition,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     @staticmethod
-    def from_convert(inner: Convert) -> "Instruction": ...
+    def from_convert(inner: Convert) -> Instruction: ...
     @staticmethod
-    def from_comparison(inner: Comparison) -> "Instruction": ...
+    def from_comparison(inner: Comparison) -> Instruction: ...
     @staticmethod
-    def from_declaration(inner: Declaration) -> "Instruction": ...
+    def from_declaration(inner: Declaration) -> Instruction: ...
     @staticmethod
-    def from_delay(inner: Delay) -> "Instruction": ...
+    def from_delay(inner: Delay) -> Instruction: ...
     @staticmethod
-    def from_exchange(inner: Exchange) -> "Instruction": ...
+    def from_exchange(inner: Exchange) -> Instruction: ...
     @staticmethod
-    def from_fence(inner: Fence) -> "Instruction": ...
+    def from_fence(inner: Fence) -> Instruction: ...
     @staticmethod
-    def from_frame_definition(inner: FrameDefinition) -> "Instruction": ...
+    def from_frame_definition(inner: FrameDefinition) -> Instruction: ...
     @staticmethod
-    def from_gate(inner: Gate) -> "Instruction": ...
+    def from_gate(inner: Gate) -> Instruction: ...
     @staticmethod
-    def from_gate_definition(inner: GateDefinition) -> "Instruction": ...
+    def from_gate_definition(inner: GateDefinition) -> Instruction: ...
     @staticmethod
-    def from_include(inner: Include) -> "Instruction": ...
+    def from_include(inner: Include) -> Instruction: ...
     @staticmethod
-    def from_jump(inner: Jump) -> "Instruction": ...
+    def from_jump(inner: Jump) -> Instruction: ...
     @staticmethod
-    def from_jump_when(inner: JumpWhen) -> "Instruction": ...
+    def from_jump_when(inner: JumpWhen) -> Instruction: ...
     @staticmethod
-    def from_jump_unless(inner: JumpUnless) -> "Instruction": ...
+    def from_jump_unless(inner: JumpUnless) -> Instruction: ...
     @staticmethod
-    def from_label(inner: Label) -> "Instruction": ...
+    def from_label(inner: Label) -> Instruction: ...
     @staticmethod
-    def from_load(inner: Load) -> "Instruction": ...
+    def from_load(inner: Load) -> Instruction: ...
     @staticmethod
     def from_measure_calibration_definition(
         inner: MeasureCalibrationDefinition,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     @staticmethod
     def from_measurement(
         inner: Measurement,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     @staticmethod
-    def from_move(inner: Move) -> "Instruction": ...
+    def from_move(inner: Move) -> Instruction: ...
     @staticmethod
-    def from_pragma(inner: Pragma) -> "Instruction": ...
+    def from_pragma(inner: Pragma) -> Instruction: ...
     @staticmethod
-    def from_pulse(inner: Pulse) -> "Instruction": ...
+    def from_pulse(inner: Pulse) -> Instruction: ...
     @staticmethod
-    def from_raw_capture(inner: RawCapture) -> "Instruction": ...
+    def from_raw_capture(inner: RawCapture) -> Instruction: ...
     @staticmethod
-    def from_set_frequency(inner: SetFrequency) -> "Instruction": ...
+    def from_set_frequency(inner: SetFrequency) -> Instruction: ...
     @staticmethod
-    def from_set_phase(inner: SetPhase) -> "Instruction": ...
+    def from_set_phase(inner: SetPhase) -> Instruction: ...
     @staticmethod
-    def from_set_scale(inner: SetScale) -> "Instruction": ...
+    def from_set_scale(inner: SetScale) -> Instruction: ...
     @staticmethod
-    def from_shift_frequency(inner: ShiftFrequency) -> "Instruction": ...
+    def from_shift_frequency(inner: ShiftFrequency) -> Instruction: ...
     @staticmethod
-    def from_shift_phase(inner: ShiftPhase) -> "Instruction": ...
+    def from_shift_phase(inner: ShiftPhase) -> Instruction: ...
     @staticmethod
-    def from_unary_logic(inner: UnaryLogic) -> "Instruction": ...
+    def from_unary_logic(inner: UnaryLogic) -> Instruction: ...
     @staticmethod
-    def from_store(inner: Store) -> "Instruction": ...
+    def from_store(inner: Store) -> Instruction: ...
     @staticmethod
-    def from_swap_phases(inner: SwapPhases) -> "Instruction": ...
+    def from_swap_phases(inner: SwapPhases) -> Instruction: ...
     @staticmethod
-    def from_reset(inner: Reset) -> "Instruction": ...
+    def from_reset(inner: Reset) -> Instruction: ...
     @staticmethod
     def from_waveform_definition(
         inner: WaveformDefinition,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     def as_arithmetic(self) -> Optional[Arithmetic]: ...
     def to_arithmetic(self) -> Arithmetic: ...
     def as_binary_logic(self) -> Optional[BinaryLogic]: ...
     def to_binary_logic(self) -> BinaryLogic: ...
     def as_convert(self) -> Optional[Convert]: ...
     def to_convert(self) -> Convert: ...
     def as_comparison(self) -> Optional[Comparison]: ...
@@ -363,96 +357,95 @@
     def as_store(self) -> Optional[Store]: ...
     def to_store(self) -> Store: ...
     def as_swap_phases(self) -> Optional[SwapPhases]: ...
     def to_swap_phases(self) -> SwapPhases: ...
     def as_waveform_definition(self) -> Optional[WaveformDefinition]: ...
     def to_waveform_definition(self) -> WaveformDefinition: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
+        """Attempt to convert the instruction to a valid Quil string. Raises an exception if the instruction can't be converted to valid Quil."""
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class ArithmeticOperand:
-    """
-    A Quil arithmetic operand.
+    """A Quil arithmetic operand.
 
     # Variants:
     - ``literal_integer``: An integer literal.
     - ``literal_real``: A real numbered literal.
     - ``memory_reference``: A Quil ``MemoryReference``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the operand is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``ArithmeticOperand`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[int, float, MemoryReference]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_literal_integer(self) -> bool: ...
     def is_literal_real(self) -> bool: ...
     def is_memory_reference(self) -> bool: ...
     def as_literal_integer(self) -> Optional[int]: ...
     def as_literal_real(self) -> Optional[float]: ...
     def as_memory_reference(self) -> Optional[MemoryReference]: ...
     def to_literal_integer(self) -> int: ...
     def to_literal_real(self) -> float: ...
     def to_memory_reference(self) -> MemoryReference: ...
     @staticmethod
-    def from_literal_integer(inner: int) -> "ArithmeticOperand": ...
+    def from_literal_integer(inner: int) -> ArithmeticOperand: ...
     @staticmethod
-    def from_literal_real(inner: float) -> "ArithmeticOperand": ...
+    def from_literal_real(inner: float) -> ArithmeticOperand: ...
     @staticmethod
     def from_memory_reference(
         inner: MemoryReference,
-    ) -> "ArithmeticOperand": ...
+    ) -> ArithmeticOperand: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class ArithmeticOperator(Enum):
     Add = "Add"
     Subtract = "Subtract"
     Divide = "Divide"
     Multiply = "Multiply"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Arithmetic:
     def __new__(
         cls,
         operator: ArithmeticOperator,
         destination: ArithmeticOperand,
@@ -467,89 +460,88 @@
     @destination.setter
     def destination(self, operand: ArithmeticOperand) -> None: ...
     @property
     def source(self) -> ArithmeticOperand: ...
     @source.setter
     def source(self, operand: ArithmeticOperand) -> None: ...
     def to_quil(self) -> str:
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
-        ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original. Should be used by passing
+        an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class BinaryOperand:
-    """
-    A Quil binary operand.
+    """A Quil binary operand.
 
     # Variants:
     - ``literal_integer``: An integer literal.
     - ``memory_reference``: A Quil ``MemoryReference``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the operand is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``BinaryOperand`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[int, MemoryReference]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_literal_integer(self) -> bool: ...
     def is_memory_reference(self) -> bool: ...
     def as_literal_integer(self) -> Optional[int]: ...
     def as_memory_reference(self) -> Optional[MemoryReference]: ...
     def to_literal_integer(self) -> int: ...
     def to_memory_reference(self) -> MemoryReference: ...
     @staticmethod
-    def from_literal_integer(inner: int) -> "BinaryOperand": ...
+    def from_literal_integer(inner: int) -> BinaryOperand: ...
     @staticmethod
     def from_memory_reference(
         inner: MemoryReference,
-    ) -> "BinaryOperand": ...
+    ) -> BinaryOperand: ...
     def to_quil(self) -> str:
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
-        ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class BinaryOperator(Enum):
     And = "AND"
     Ior = "IOR"
     Xor = "XOR"
     def to_quil(self) -> str:
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
-        ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class BinaryOperands:
     def __new__(
         cls,
         memory_reference: MemoryReference,
         operand: BinaryOperand,
@@ -574,156 +566,173 @@
     @operator.setter
     def operator(self, operator: BinaryOperator) -> None: ...
     @property
     def operands(self) -> BinaryOperands: ...
     @operands.setter
     def operands(self, operands: BinaryOperands) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Convert:
     def __new__(cls, destination: MemoryReference, source: MemoryReference) -> Self: ...
     @property
     def destination(self) -> MemoryReference: ...
     @destination.setter
     def destination(self, destination: MemoryReference) -> None: ...
     @property
     def source(self) -> MemoryReference: ...
     @source.setter
     def source(self, source: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Move:
     def __new__(cls, destination: MemoryReference, source: ArithmeticOperand) -> Self: ...
     @property
     def destination(self) -> MemoryReference: ...
     @destination.setter
     def destination(self, destination: MemoryReference) -> None: ...
     @property
     def source(self) -> ArithmeticOperand: ...
     @source.setter
     def source(self, source: ArithmeticOperand) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Exchange:
     def __new__(cls, left: MemoryReference, right: MemoryReference) -> Self: ...
     @property
     def left(self) -> MemoryReference: ...
     @left.setter
     def left(self, left: MemoryReference) -> None: ...
     @property
     def right(self) -> MemoryReference: ...
     @right.setter
     def right(self, right: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class ComparisonOperand:
-    """
-    A Quil binary operand.
+    """A Quil binary operand.
 
     # Variants:
     - ``literal_integer``: An integer literal.
     - ``literal_real``: A floating point literal.
     - ``memory_reference``: A Quil ``MemoryReference``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the operand is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``BinaryOperand`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[int, float, MemoryReference]:
-        """
-        Returns the inner value of the variant.
-        """
+        """Returns the inner value of the variant."""
         ...
     def is_literal_integer(self) -> bool: ...
     def is_literal_real(self) -> bool: ...
     def is_memory_reference(self) -> bool: ...
     def as_literal_integer(self) -> Optional[int]: ...
     def as_literal_real(self) -> Optional[float]: ...
     def as_memory_reference(self) -> Optional[MemoryReference]: ...
     def to_literal_integer(self) -> int: ...
     def to_literal_real(self) -> float: ...
     def to_memory_reference(self) -> MemoryReference: ...
     @staticmethod
-    def from_literal_integer(inner: int) -> "ComparisonOperand": ...
+    def from_literal_integer(inner: int) -> ComparisonOperand: ...
     @staticmethod
-    def from_literal_real(inner: float) -> "ComparisonOperand": ...
+    def from_literal_real(inner: float) -> ComparisonOperand: ...
     @staticmethod
     def from_memory_reference(
         inner: MemoryReference,
-    ) -> "ComparisonOperand": ...
+    ) -> ComparisonOperand: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class ComparisonOperator(Enum):
     Equal = "EQUAL"
     GreaterThanOrEqual = "GREATERTHANOREQUAL"
     GreaterThan = "GREATERTHAN"
@@ -743,68 +752,78 @@
     @property
     def operands(
         self,
     ) -> Tuple[MemoryReference, MemoryReference, ComparisonOperand]: ...
     @operands.setter
     def operands(self, operands: Tuple[MemoryReference, MemoryReference, ComparisonOperand]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class UnaryOperator(Enum):
     Neg = "NEG"
     Not = "NOT"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class UnaryLogic:
     def __new__(cls, operator: UnaryOperator, operand: MemoryReference) -> Self: ...
     @property
     def operator(self) -> UnaryOperator: ...
     @operator.setter
     def operator(self, operator: UnaryOperator) -> None: ...
     @property
     def operand(self) -> MemoryReference: ...
     @operand.setter
     def operand(self, operand: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Calibration:
     def __new__(
         cls,
         name: str,
@@ -830,26 +849,31 @@
     @instructions.setter
     def instructions(self, instructions: Sequence[Instruction]) -> None: ...
     @property
     def modifiers(self) -> List[GateModifier]: ...
     @modifiers.setter
     def modifiers(self, modifiers: Sequence[GateModifier]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class MeasureCalibrationDefinition:
     def __new__(
         cls,
         qubit: Optional[Qubit],
@@ -865,26 +889,31 @@
     @parameter.setter
     def parameter(self, parameter: str) -> None: ...
     @property
     def instructions(self) -> List[Instruction]: ...
     @instructions.setter
     def instructions(self, instructions: Sequence[Instruction]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class CircuitDefinition:
     def __new__(
         cls,
         name: str,
@@ -905,26 +934,31 @@
     @qubit_variables.setter
     def qubit_variables(self, qubit_variables: Sequence[str]) -> None: ...
     @property
     def instructions(self) -> List[Instruction]: ...
     @instructions.setter
     def instructions(self, instructions: Sequence[Instruction]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Offset:
     def __new__(
         cls,
         offset: int,
@@ -935,23 +969,23 @@
     @offset.setter
     def offset(self, offset: int) -> None: ...
     @property
     def data_type(self) -> ScalarType: ...
     @data_type.setter
     def data_type(self, data_type: ScalarType) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Sharing:
     def __new__(
         cls,
         name: str,
         offsets: Sequence[Offset],
@@ -976,110 +1010,112 @@
     @size.setter
     def size(self, vector: Vector) -> None: ...
     @property
     def sharing(self) -> Optional[Sharing]: ...
     @sharing.setter
     def sharing(self, sharing: Optional[Sharing]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Vector:
     def __new__(cls, data_type: ScalarType, length: int) -> Self: ...
     @property
     def data_type(self) -> ScalarType: ...
     @data_type.setter
     def data_type(self, data_type: ScalarType) -> None: ...
     @property
     def length(self) -> int: ...
     @length.setter
     def length(self, data_type: int) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class ScalarType(Enum):
     Bit = "BIT"
     Integer = "INTEGER"
     Octet = "OCTET"
     Real = "REAL"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class AttributeValue:
-    """
-    A frame attribute value.
+    """A frame attribute value.
 
     # Variants:
     - ``string``: A string attribute containing a ``str``.
     - ``expression``: An expression attribute containing an ``Expression``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the ``AttributeValue`` is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``AttributeValue`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[str, Expression]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_string(self) -> bool: ...
     def is_expression(self) -> bool: ...
     @staticmethod
-    def from_string(inner: str) -> "AttributeValue": ...
+    def from_string(inner: str) -> AttributeValue: ...
     @staticmethod
-    def from_expression(inner: Expression) -> "AttributeValue": ...
+    def from_expression(inner: Expression) -> AttributeValue: ...
     def as_string(self) -> Optional[str]: ...
     def to_string(self) -> str: ...
     def as_expression(self) -> Optional[Expression]: ...
     def to_expression(self) -> Expression: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class FrameDefinition:
     def __new__(
         cls,
         identifier: FrameIdentifier,
         attributes: Dict[str, AttributeValue],
@@ -1089,49 +1125,54 @@
     @identifier.setter
     def identifier(self, identifier: FrameIdentifier) -> None: ...
     @property
     def attributes(self) -> Dict[str, AttributeValue]: ...
     @attributes.setter
     def attributes(self, identifier: Dict[str, AttributeValue]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class FrameIdentifier:
     def __new__(cls, name: str, qubits: Sequence[Qubit]) -> Self: ...
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def qubits(self) -> List[Qubit]: ...
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Capture:
     def __new__(
         cls,
         blocking: bool,
         frame: FrameIdentifier,
@@ -1151,26 +1192,31 @@
     @memory_reference.setter
     def memory_reference(self, memory_reference: MemoryReference) -> None: ...
     @property
     def waveform(self) -> WaveformInvocation: ...
     @waveform.setter
     def waveform(self, waveform: WaveformInvocation) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Pulse:
     def __new__(
         cls,
         blocking: bool,
@@ -1186,26 +1232,31 @@
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def waveform(self) -> WaveformInvocation: ...
     @waveform.setter
     def waveform(self, waveform: WaveformInvocation) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class RawCapture:
     def __new__(
         cls,
         blocking: bool,
@@ -1226,205 +1277,240 @@
     @duration.setter
     def duration(self, duration: Expression) -> None: ...
     @property
     def memory_reference(self) -> MemoryReference: ...
     @memory_reference.setter
     def memory_reference(self, memory_reference: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SetFrequency:
     def __new__(cls, frame: FrameIdentifier, frequency: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def frequency(self) -> Expression: ...
     @frequency.setter
     def frequency(self, frequency: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SetPhase:
     def __new__(cls, frame: FrameIdentifier, phase: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def phase(self) -> Expression: ...
     @phase.setter
     def phase(self, phase: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SetScale:
     def __new__(cls, frame: FrameIdentifier, phase: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def scale(self) -> Expression: ...
     @scale.setter
     def scale(self, scale: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class ShiftFrequency:
     def __new__(cls, frame: FrameIdentifier, frequency: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def frequency(self) -> Expression: ...
     @frequency.setter
     def frequency(self, frequency: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class ShiftPhase:
     def __new__(cls, frame: FrameIdentifier, phase: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def phase(self) -> Expression: ...
     @phase.setter
     def phase(self, phase: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SwapPhases:
     def __new__(cls, frame_1: FrameIdentifier, frame_2: FrameIdentifier) -> Self: ...
     @property
     def frame_1(self) -> FrameIdentifier: ...
     @frame_1.setter
     def frame_1(self, frame_1: FrameIdentifier) -> None: ...
     @property
     def frame_2(self) -> FrameIdentifier: ...
     @frame_2.setter
     def frame_2(self, frame_2: FrameIdentifier) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class GateError(ValueError):
-    """An error that may occur when performing operations on a ``Gate``"""
+    """An error that may occur when performing operations on a ``Gate``."""
 
     ...
 
 @final
 class GateModifier(Enum):
     Controlled = "CONTROLLED"
     Dagger = "DAGGER"
     Forked = "FORKED"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Gate:
     def __new__(
         cls,
         name: str,
         parameters: Sequence[Expression],
@@ -1444,67 +1530,63 @@
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     @property
     def modifiers(self) -> List[GateModifier]: ...
     @modifiers.setter
     def modifiers(self, modifiers: Sequence[GateModifier]) -> None: ...
     def dagger(self) -> Self:
-        """
-        Returns a copy of the gate with the ``DAGGER`` modifier added to it.
-        """
+        """Returns a copy of the gate with the ``DAGGER`` modifier added to it."""
         ...
     def controlled(self, control_qubit: Qubit) -> Self:
-        """
-        Returns a copy of the gate with the ``CONTROLLED`` modifier added to it.
-        """
+        """Returns a copy of the gate with the ``CONTROLLED`` modifier added to it."""
     def forked(self, fork_qubit: Qubit, alt_params: Sequence[Expression]) -> Self:
-        """
-        Returns a copy of the gate with the ``FORKED`` modifier added to it.
+        """Returns a copy of the gate with the ``FORKED`` modifier added to it.
 
         Raises a ``GateError`` if the number of provided alternate parameters don't
         equal the number of existing parameters.
         """
         ...
     def to_unitary_mut(self, n_qubits: int) -> NDArray[np.complex_]:
-        """
-        Lift a Gate to the full `n_qubits`-qubit Hilbert space.
+        """Lift a Gate to the full `n_qubits`-qubit Hilbert space.
 
         Returns a ``GateError` if any of the parameters of this gate are
         non-constant, if any of the qubits are variable, if the name of this
         gate is unknown, or if there are an unexpected number of parameters.
         """
         ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class PauliGate(Enum):
     I = "I"
     X = "X"
     Y = "Y"
     Z = "Z"
     @staticmethod
-    def parse(input: str) -> "PauliGate":
-        """
-        Parses a ``PauliGate`` from a string. Raises a ``ParseEnumError`` if the
-        string isn't a valid Pauli word.
-        """
+    def parse(input: str) -> PauliGate:
+        """Parses a ``PauliGate`` from a string. Raises a ``ParseEnumError`` if the string isn't a valid Pauli word."""
         ...
 
 class PauliTerm:
     def __new__(
         cls,
         arguments: Sequence[Tuple[PauliGate, str]],
         expression: Expression,
@@ -1527,58 +1609,55 @@
     @property
     def terms(self) -> List[PauliTerm]: ...
     @terms.setter
     def terms(self, terms: Sequence[PauliTerm]) -> None: ...
 
 @final
 class GateSpecification:
-    """
-    A specification for a gate definition.
+    """A specification for a gate definition.
 
     # Variants:
-    - ``matrix``: A gate specificied by a matrix of ``Expression``s representing a unitary operation.
+    - ``matrix``: A gate specified by a matrix of ``Expression``s representing a unitary operation.
     - ``permutation``: A gate specified by a vector of integers that defines a permutation.
 
     Methods (for each variant):
     - is_*: Returns ``True`` if the inner type is of that variant.
     - as_*: Returns the inner data if it is the given variant, ``None`` otherwise.
     - to_*: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - from_*: Creates a new ``GateSpecification`` using an instance of the inner type for the variant.
     """
 
     def inner(self) -> Union[List[List[Expression]], List[int], PauliSum]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_matrix(self) -> bool: ...
     def is_permutation(self) -> bool: ...
     def is_pauli_sum(self) -> bool: ...
     def as_matrix(self) -> Optional[List[List[Expression]]]: ...
     def to_matrix(self) -> List[List[Expression]]: ...
     def as_permutation(self) -> Optional[List[int]]: ...
     def to_permutation(self) -> List[int]: ...
     def as_pauli_sum(self) -> Optional[PauliSum]: ...
     def to_pauli_sum(self) -> PauliSum: ...
     @staticmethod
-    def from_matrix(inner: Sequence[Sequence[Expression]]) -> "GateSpecification": ...
+    def from_matrix(inner: Sequence[Sequence[Expression]]) -> GateSpecification: ...
     @staticmethod
-    def from_permutation(inner: Sequence[int]) -> "GateSpecification": ...
+    def from_permutation(inner: Sequence[int]) -> GateSpecification: ...
     @staticmethod
-    def from_pauli_sum(inner: PauliSum) -> "GateSpecification": ...
+    def from_pauli_sum(inner: PauliSum) -> GateSpecification: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class GateDefinition:
     def __new__(
         cls,
         name: str,
         parameters: Sequence[str],
@@ -1593,105 +1672,112 @@
     @parameters.setter
     def parameters(self, parameters: Sequence[str]) -> None: ...
     @property
     def specification(self) -> GateSpecification: ...
     @specification.setter
     def specification(self, specification: GateSpecification) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class Qubit:
-    """
-    A Qubit
+    """A Qubit.
 
     # Variants:
     - ``fixed``: A qubit represented as a fixed integer index.
     - ``variable``: A qubit represented by a name.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the inner type is of that variant.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``Qubit`` using an instance of the inner type for the variant.
     """
 
     def inner(self) -> Union[int, str]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_fixed(self) -> bool: ...
     def is_variable(self) -> bool: ...
     def is_placeholder(self) -> bool: ...
     def as_fixed(self) -> Optional[int]: ...
     def to_fixed(self) -> int: ...
     def as_variable(self) -> Optional[str]: ...
     def to_variable(self) -> str: ...
     def as_placeholder(self) -> Optional[QubitPlaceholder]: ...
     def to_placeholder(self) -> QubitPlaceholder: ...
     @staticmethod
-    def from_fixed(inner: int) -> "Qubit": ...
+    def from_fixed(inner: int) -> Qubit: ...
     @staticmethod
-    def from_variable(inner: str) -> "Qubit": ...
+    def from_variable(inner: str) -> Qubit: ...
     @staticmethod
-    def from_placeholder(inner: QubitPlaceholder) -> "Qubit": ...
+    def from_placeholder(inner: QubitPlaceholder) -> Qubit: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class QubitPlaceholder:
-    """
-    A qubit that can be used as a placeholder. Must be resolved before converting
-    a program to valid Quil. See ``quil.program.Program#resolve_placeholders``.
+    """A qubit that can be used as a placeholder.
+
+    Placeholders must be resolved before converting a program to valid Quil. See ``quil.program.Program#resolve_placeholders``.
     """
 
     def __new__(cls) -> Self: ...
     def __lt__(self, other: QubitPlaceholder) -> bool: ...
 
 class Reset:
     def __new__(cls, qubit: Optional[Qubit]) -> Self: ...
     @property
     def qubit(self) -> Optional[Qubit]: ...
     @qubit.setter
     def qubit(self, qubit: Optional[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Delay:
     def __new__(cls, duration: Expression, frame_names: Sequence[str], qubits: Sequence[Qubit]) -> Self: ...
     @property
     def duration(self) -> Expression: ...
@@ -1702,112 +1788,125 @@
     @frame_names.setter
     def frame_names(self, frame_names: Sequence[str]) -> None: ...
     @property
     def qubits(self) -> List[Qubit]: ...
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Fence:
     def __new__(cls, qubits: Sequence[Qubit]) -> Self: ...
     @property
     def qubits(self) -> List[Qubit]: ...
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class PragmaArgument:
-    """
+    """A PRAGMA argument.
 
-    # Variants:
+    Variants:
     - ``identifier``: A Pragma argument defined by a Quil identifier
     - ``integer``: A Pragma argument defined by an integer
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the inner type is of that variant.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``PragmaArgument`` using an instance of the inner type for the variant.
     """
 
     def inner(self) -> Union[str, int]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_identifier(self) -> bool: ...
     def is_integer(self) -> bool: ...
     def as_identifier(self) -> Optional[str]: ...
     def as_integer(self) -> Optional[int]: ...
     def to_identifier(self) -> str: ...
     def to_integer(self) -> int: ...
     @staticmethod
-    def from_identifier(inner: str) -> "PragmaArgument": ...
+    def from_identifier(inner: str) -> PragmaArgument: ...
     @staticmethod
-    def from_integer(inner: int) -> "PragmaArgument": ...
+    def from_integer(inner: int) -> PragmaArgument: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Include:
     def __new__(cls, filename: str) -> Self: ...
     @property
     def filename(self) -> str: ...
     @filename.setter
     def filename(self, filename: str) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Pragma:
     def __new__(cls, name: str, arguments: Sequence[PragmaArgument], data: Optional[str]) -> Self: ...
     @property
     def name(self) -> str: ...
@@ -1818,85 +1917,95 @@
     @arguments.setter
     def arguments(self, arguments: Sequence[PragmaArgument]) -> None: ...
     @property
     def data(self) -> Optional[str]: ...
     @data.setter
     def data(self, data: Optional[str]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Measurement:
     def __new__(cls, qubit: Qubit, target: Optional[MemoryReference]) -> Self: ...
     @property
     def qubit(self) -> Qubit: ...
     @qubit.setter
     def qubit(self, qubit: Qubit) -> None: ...
     @property
     def target(self) -> Optional[MemoryReference]: ...
     @target.setter
     def target(self, target: Optional[MemoryReference]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class ParseMemoryReferenceError(ValueError):
-    """Errors that may occur while parsing a ``MemoryReference``"""
+    """Errors that may occur while parsing a ``MemoryReference``."""
 
 class MemoryReference:
     def __new__(cls, name: str, index: int) -> Self: ...
     @staticmethod
-    def parse(input: str) -> "MemoryReference":
-        """
-        Parses a ``MemoryReference`` from a string. Raises a ``ParseMemoryReference`` error if the
-        string isn't a valid Quil memory reference.
+    def parse(input: str) -> MemoryReference:
+        """Parses a ``MemoryReference`` from a string.
+
+        Raises a ``ParseMemoryReference`` error if the string isn't a valid Quil memory reference.
         """
         ...
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def index(self) -> int: ...
     @index.setter
     def index(self, index: int) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Load:
     def __new__(cls, destination: MemoryReference, source: str, offset: MemoryReference) -> Self: ...
     @property
     def destination(self) -> MemoryReference: ...
     @destination.setter
@@ -1906,26 +2015,31 @@
     @source.setter
     def source(self, source: str) -> None: ...
     @property
     def offset(self) -> MemoryReference: ...
     @offset.setter
     def offset(self, offset: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Store:
     def __new__(cls, destination: str, offset: MemoryReference, source: ArithmeticOperand) -> Self: ...
     @property
     def destination(self) -> str: ...
@@ -1936,26 +2050,31 @@
     @offset.setter
     def offset(self, offset: MemoryReference) -> None: ...
     @property
     def source(self) -> ArithmeticOperand: ...
     @source.setter
     def source(self, source: ArithmeticOperand) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Waveform:
     def __new__(cls, matrix: Sequence[Expression], parameters: Sequence[str]) -> Self: ...
     @property
     def matrix(self) -> List[Expression]: ...
@@ -1973,117 +2092,124 @@
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def definition(self) -> Waveform: ...
     @definition.setter
     def definition(self, definition: Waveform) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class WaveformInvocation:
     def __new__(cls, name: str, parameters: Dict[str, Expression]) -> Self: ...
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def parameters(self) -> Dict[str, Expression]: ...
     @parameters.setter
     def parameters(self, parameters: Dict[str, Expression]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Label:
     def __new__(cls, target: Target) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class Target:
-    """
-    Represents a Quil target.
+    """Represents a Quil target.
 
     # Variants:
     - ``fixed``: A fixed target defined by a Quil identifier
     - ``placeholder``: A placeholder target that can be assigned a new name at a later time.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the inner type is of that variant.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``PragmaArgument`` using an instance of the inner type for the variant.
     """
 
-    def __new__(cls, inner: Union[str, TargetPlaceholder]) -> "Target": ...
+    def __new__(cls, inner: Union[str, TargetPlaceholder]) -> Target: ...
     @staticmethod
-    def from_fixed(inner: str) -> "Target": ...
+    def from_fixed(inner: str) -> Target: ...
     @staticmethod
-    def from_placeholder(inner: TargetPlaceholder) -> "Target": ...
+    def from_placeholder(inner: TargetPlaceholder) -> Target: ...
     def is_fixed(self) -> bool: ...
     def is_placeholder(self) -> bool: ...
     def as_fixed(self) -> Optional[str]: ...
     def as_placeholder(self) -> Optional[TargetPlaceholder]: ...
     def to_fixed(self) -> str: ...
     def to_placeholder(self) -> TargetPlaceholder: ...
     def inner(self) -> Union[str, TargetPlaceholder]: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class TargetPlaceholder:
-    """
-    A placeholder target that must be assigned a fixed name before creating a program
-    with valid quil.
+    """A placeholder target that must be assigned a fixed name before creating a program with valid quil.
 
     See ``quil.program.Program#resolve_placeholders`` for more information.
     """
 
     def __new__(cls, base_target: str) -> Self: ...
     @property
     def base_label(self) -> str: ...
@@ -2091,73 +2217,88 @@
 class Jump:
     def __new__(cls, target: Target) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class JumpWhen:
     def __new__(cls, target: Target, condition: MemoryReference) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     @property
     def condition(self) -> MemoryReference: ...
     @condition.setter
     def condition(self, condition: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class JumpUnless:
     def __new__(cls, target: Target, condition: MemoryReference) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     @property
     def condition(self) -> MemoryReference: ...
     @condition.setter
     def condition(self, condition: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
```

### Comparing `quil-0.9.0rc0/quil-py/quil/program/__init__.pyi` & `quil-0.9.1rc0/quil-py/quil/program/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from typing import Dict, FrozenSet, Set, final, List, Optional, Sequence, Callable
+from typing import Callable, Dict, FrozenSet, List, Optional, Sequence, Set, final
 
 import numpy as np
 from numpy.typing import NDArray
+from typing_extensions import Self
+
 from quil.instructions import (
     AttributeValue,
     Calibration,
     Declaration,
     FrameIdentifier,
     Gate,
     GateDefinition,
     Instruction,
     MeasureCalibrationDefinition,
     Measurement,
     MemoryReference,
     Qubit,
+    QubitPlaceholder,
     Sharing,
     Target,
+    TargetPlaceholder,
     Vector,
     Waveform,
-    TargetPlaceholder,
-    QubitPlaceholder,
 )
 
 @final
 class Program:
     @staticmethod
     def __new__(cls) -> "Program": ...
     @property
@@ -47,95 +49,78 @@
     @property
     def memory_regions(self) -> Dict[str, MemoryRegion]: ...
     @memory_regions.setter
     def memory_regions(self, memory_regions: Dict[str, MemoryRegion]): ...
     @property
     def declarations(self) -> Dict[str, Declaration]: ...
     def dagger(self) -> "Program":
-        """
-        Creates a new conjugate transpose of the ``Program`` by reversing the order of gate
-        instructions and applying the DAGGER modifier to each.
+        """Creates a new conjugate transpose of the ``Program`` by reversing the order of gate instructions and applying the DAGGER modifier to each.
 
         Raises a ``GateError`` if any of the instructions in the program are not a ``Gate`
         """
         ...
     def expand_calibrations(self) -> "Program":
-        """
-        Expand any instructions in the program which have a matching calibration, leaving the others
-        unchanged. Recurses though each instruction while ensuring there is no cycle in the expansion
-        graph (i.e. no calibration expands directly or indirectly into itself)
+        """Expand any instructions in the program which have a matching calibration, leaving the others unchanged.
+
+        Recurses though each instruction while ensuring there is no cycle in the expansion graph (i.e. no calibration
+        expands directly or indirectly into itself)
         """
         ...
     def into_simplified(self) -> "Program":
-        """
-        Simplify this program into a new [`Program`] which contains only instructions
-        and definitions which are executed; effectively, perform dead code removal.
+        """Simplify this program into a new `Program` which contains only instructions and definitions which are executed; effectively, perform dead code removal.
 
         Removes:
         - All calibrations, following calibration expansion
         - Frame definitions which are not used by any instruction such as `PULSE` or `CAPTURE`
         - Waveform definitions which are not used by any instruction
 
         When a valid program is simplified, it remains valid.
         """
         ...
     def get_used_qubits(self) -> Set[Qubit]:
-        """
-        Returns a set consisting of every Qubit that is used in the program.
-        """
+        """Returns a set consisting of every Qubit that is used in the program."""
         ...
     def add_instruction(self, instruction: Instruction):
-        """
-        Add an instruction to the end of the program.
-        """
+        """Add an instruction to the end of the program."""
         ...
     def add_instructions(self, instructions: Sequence[Instruction]):
-        """
-        Add a list of instructions to the end of the program.
-        """
+        """Add a list of instructions to the end of the program."""
         ...
     @staticmethod
     def parse(input: str) -> "Program":
-        """
-        Parses the given Quil string and returns a new ``Program``.
+        """Parses the given Quil string and returns a new ``Program``.
+
         Raises a ``ProgramError`` if the given string isn't valid Quil.
         """
     def to_instructions(self) -> Sequence[Instruction]: ...
     def to_unitary(self, n_qubits: int) -> NDArray[np.complex_]: ...
     def copy(self) -> "Program":
-        """
-        Creates a clone of this ``Program``.
-        """
+        """Creates a clone of this ``Program``."""
         ...
     def clone_without_body_instructions(self) -> "Program":
-        """
-        Creates a clone of this ``Program`` with an empty body instructions list.
-        """
+        """Creates a clone of this ``Program`` with an empty body instructions list."""
     def __add__(self, rhs: Program) -> Program: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def filter_instructions(self, predicate: Callable[[Instruction], bool]) -> "Program":
-        """
-        Return a new ``Program`` containing only the instructions for which ``predicate`` returns ``True``.
-        """
+        """Return a new ``Program`` containing only the instructions for which ``predicate`` returns ``True``."""
         ...
     def wrap_in_loop(
         self, loop_count_reference: MemoryReference, start_target: Target, end_target: Target, iterations: int
     ) -> "Program":
-        """
-        Return a copy of the `Program` wrapped in a loop that repeats ``iterations`` times.
+        """Return a copy of the `Program` wrapped in a loop that repeats ``iterations`` times.
 
         The loop is constructed by wrapping the body of the program in classical Quil instructions.
         The given ``loop_count_reference`` must refer to an INTEGER memory region. The value at the
         reference given will be set to ``iterations`` and decremented in the loop. The loop will
         terminate when the reference reaches 0. For this reason your program should not itself
         modify the value at the reference unless you intend to modify the remaining number of
         iterations (i.e. to break the loop).
@@ -145,54 +130,51 @@
         used elsewhere in the program.
 
         If `iterations` is 0, then a copy of the program is returned without any changes. Raises a
         `TypeError` if `iterations` is negative.
         """
         ...
     def resolve_placeholders(self) -> None:
-        """
-        Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program using default resolvers.
+        """Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program using default resolvers.
 
         The default resolver will be used to generate a unique value for that placeholder within the scope of
         the program using an auto-incrementing value (for qubit) or suffix (for target)
         while ensuring that unique value is not already in use within the program.
         """
         ...
     def resolve_placeholders_with_custom_resolvers(
         self,
         *,
         target_resolver: Optional[Callable[[TargetPlaceholder], Optional[str]]] = None,
         qubit_resolver: Optional[Callable[[QubitPlaceholder], Optional[int]]] = None,
     ):
-        """
-        Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program such that the resolved values
-        will remain unique to that placeholder within the scope of the program.
+        """Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program.
+
+        The resolved values will remain unique to that placeholder within the scope of the program.
 
         If you provide ``target_resolver`` and/or ``qubit_resolver``, those will be used to resolve those values respectively.
         If your resolver returns `None` for a particular placeholder, it will not be replaced but will be left as a placeholder.
 
         If you do not provide a resolver for a placeholder, a default resolver will be used which will generate a unique value
         for that placeholder within the scope of the program using an auto-incrementing value (for qubit) or suffix (for target)
         while ensuring that unique value is not already in use within the program.
         """
         ...
     def control_flow_graph(self) -> "ControlFlowGraph":
-        """
-        Return the `control flow graph`_ of the program.
+        """Return the `control flow graph`_ of the program.
 
         .. _control flow graph: https://en.wikipedia.org/wiki/Control-flow_graph
         """
 
-@final
 class BasicBlock:
-    def as_schedule_seconds(self, program: Program) -> ScheduleSeconds:
-        """
-        Return the ``ScheduleSeconds`` representing the timing of the instructions within the block.
+    def __new__(cls, instance: "BasicBlock") -> Self:
+        """Create a new instance of a `BasicBlock` (or a subclass) using an existing instance."""
 
-        This schedule is computed by:
+    def as_schedule_seconds(self, program: Program) -> ScheduleSeconds:
+        """Return the ``ScheduleSeconds`` representing the timing of the instructions within the block.
 
         * Expanding each instruction within the block using the program's calibration definitions
         * Resolving the `ScheduleSeconds` of the expanded instructions
         * Mapping calibrated instructions back to the original instructions within this block, such that the
           block's instruction is represented as a timespan encompassing all of its expanded instructions
 
         Note: the schedule will not include instructions with zero duration (such as `FENCE`).
@@ -253,33 +235,27 @@
                 A 0
                 B 0 1
 
         `B 0` will be scheduled from time 0 to time 2, because its inner `FENCE` is scheduled for time 0.
         This may be unexpected if the user expects to see only the timing of the inner `PULSE`.
         """
     def gate_depth(self, gate_minimum_qubit_count: int) -> int:
-        """
-        Returns the length of the longest path from an initial instruction (one with no prerequisite instructions) to a final
-        instruction (one with no dependent instructions), where the length of a path is the number of gate instructions in the path.
+        """Returns the length of the longest path from an initial instruction (one with no prerequisite instructions) to a final instruction (one with no dependent instructions), where the length of a path is the number of gate instructions in the path.
 
         :param gate_minimum_qubit_count: The minimum number of qubits in a gate for it to be counted in the depth.
         """
     def label(self) -> Optional[Target]:
-        """
-        Return the label of the block, if any. This is used to target this block in control flow.
-        """
+        """Return the label of the block, if any. This is used to target this block in control flow."""
     def instructions(self) -> List[Instruction]:
-        """
-        Return a list of the instructions in the block, in order of definition.
+        """Return a list of the instructions in the block, in order of definition.
 
         This does not include the label or terminator instructions.
         """
     def terminator(self) -> Optional[Instruction]:
-        """
-        Return the control flow terminator instruction of the block, if any.
+        """Return the control flow terminator instruction of the block, if any.
 
         If this is ``None``, the implicit behavior is to "continue" to the subsequent block.
         """
 
 @final
 class CalibrationSet:
     @staticmethod
@@ -289,184 +265,141 @@
         measure_calibration_definitions: Sequence[MeasureCalibrationDefinition],
     ) -> "CalibrationSet": ...
     @property
     def calibrations(self) -> List[Calibration]: ...
     @property
     def measure_calibrations(self) -> List[MeasureCalibrationDefinition]: ...
     def expand(self, instruction: Instruction, previous_calibrations: Sequence[Instruction]) -> List[Instruction]:
-        """
-        Given an instruction, return the instructions to which it is expanded if there is a match.
+        """Given an instruction, return the instructions to which it is expanded if there is a match.
+
         Recursively calibrate instructions, returning an error if a calibration directly or indirectly
         expands into itself.
         """
     ...
 
     def get_match_for_measurement(self, measurement: Measurement) -> Optional[MeasureCalibrationDefinition]:
-        """
-        Returns the last-specified ``MeasureCalibrationDefinition`` that matches the target
-        qubit (if any), or otherwise the last-specified one that specified no qubit.
-        """
+        """Returns the last-specified ``MeasureCalibrationDefinition`` that matches the target qubit (if any), or otherwise the last-specified one that specified no qubit."""
         ...
     def get_match_for_gate(self, gate: Gate) -> Optional[Calibration]:
-        """
-        Return the final calibration which matches the gate per the QuilT specification:
+        """Return the final calibration which matches the gate per the QuilT specification.
 
         A calibration matches a gate if:
         1. It has the same name
         2. It has the same modifiers
         3. It has the same qubit count (any mix of fixed & variable)
         4. It has the same parameter count (both specified and unspecified)
         5. All fixed qubits in the calibration definition match those in the gate
         6. All specified parameters in the calibration definition match those in the gate
         """
     def __len__(self) -> int: ...
     def is_empty(self) -> bool:
         """Returns ``True`` if the ``CalibrationSet`` contains no data."""
         ...
     def insert_calibration(self, calibration: Calibration) -> Optional[Calibration]:
-        """
-        Insert another ``Calibration`` (`DEFCAL`) to the set.
+        """Insert another ``Calibration`` (`DEFCAL`) to the set.
 
         If a calibration with the same name already exists, it is overwritten and this
         function returns the previous calibration. Otherwise, None is returned.
         """
         ...
-    def insert_measurement_calibration(self, calibration: MeasureCalibrationDefinition) -> Optional[MeasureCalibrationDefinition]:
-        """
-        Add another ``MeasureCalibrationDefinition`` (`DEFCAL MEASURE`) to the set
+    def insert_measurement_calibration(
+        self, calibration: MeasureCalibrationDefinition
+    ) -> Optional[MeasureCalibrationDefinition]:
+        """Add another ``MeasureCalibrationDefinition`` (`DEFCAL MEASURE`) to the set.
 
         If a calibration with the same name already exists, it is overwritten and this
         function returns the previous calibration. Otherwise, None is returned.
         """
     def extend(self, other: CalibrationSet):
-        """
-        Append another [`CalibrationSet`] onto this one
-        """
+        """Append another [`CalibrationSet`] onto this one."""
         ...
     def to_instructions(self):
-        """
-        Return the Quil instructions which describe the contained calibrations
-        """
+        """Return the Quil instructions which describe the contained calibrations."""
         ...
 
-
-@final
 class ScheduleSecondsItem:
-    """
-    A single item within a fixed schedule, representing a single instruction within a basic block.
-    """
+    """A single item within a fixed schedule, representing a single instruction within a basic block."""
+
     @property
     def instruction_index(self) -> int:
-        """
-        The index of the instruction within the basic block.
-        """
+        """The index of the instruction within the basic block."""
     @property
     def time_span(self) -> TimeSpanSeconds:
-        """
-        The time span during which the instruction is scheduled.
-        """
-
+        """The time span during which the instruction is scheduled."""
 
-@final
 class ControlFlowGraph:
-    """
-    Representation of a control flow graph (CFG) for a Quil program.
+    """Representation of a control flow graph (CFG) for a Quil program.
 
     The CFG is a directed graph where each node is a basic block and each edge is a control flow
     transition between two basic blocks.
     """
+    def __new__(cls, instance: "ControlFlowGraph") -> Self:
+        """Create a new instance of a `ControlFlowGraph` (or a subclass) using an existing instance."""
 
-    def has_dynamic_control_flow(self) -> bool: 
-        """
-        Return ``True`` if the program has dynamic control flow, i.e. contains a conditional branch instruction.
+    def has_dynamic_control_flow(self) -> bool:
+        """Return ``True`` if the program has dynamic control flow, i.e. contains a conditional branch instruction.
 
         ``False`` does not imply that there is only one basic block in the program. Multiple basic blocks may have
         non-conditional control flow among them, in which the execution order is deterministic and does not depend
         on program state. This may be a sequence of basic blocks with fixed `JUMP`s or without explicit terminators.
         """
-    def basic_blocks(self) -> List["BasicBlock"]: 
-        """
-        Return a list of all the basic blocks in the control flow graph, in order of definition.
-        """
+    def basic_blocks(self) -> List["BasicBlock"]:
+        """Return a list of all the basic blocks in the control flow graph, in order of definition."""
 
-@final
 class ScheduleSeconds:
     def items(self) -> List[ScheduleSecondsItem]:
-        """
-        All the items in the schedule, in unspecified order.
-        """
+        """All the items in the schedule, in unspecified order."""
     def duration(self) -> float:
-        """
-        The duration of the schedule, in seconds.
+        """The duration of the schedule, in seconds.
 
         This is the maximum of the end time of all the items.
         """
 
-@final
 class TimeSpanSeconds:
-    """
-    Representation of a time span in seconds.
-    """
+    """Representation of a time span in seconds."""
+
     @property
     def start(self) -> float:
-        """
-        The start time of the time span, in seconds.
+        """The start time of the time span, in seconds.
 
         This is relative to the start of the scheduling context (such as the basic block).
         """
     @property
     def duration(self) -> float:
-        """
-        The duration of the time span, in seconds.
-        """
+        """The duration of the time span, in seconds."""
     @property
     def end(self) -> float:
-        """
-        The end time of the time span, in seconds.
+        """The end time of the time span, in seconds.
 
         This is the sum of the start time and duration.
         """
 
 @final
 class FrameSet:
     @staticmethod
     def __new__(cls) -> "FrameSet": ...
     def get(self, identifier: FrameIdentifier) -> Optional[Dict[str, AttributeValue]]:
-        """
-        Retrieve the attributes of a frame by its identifier
-        """
+        """Retrieve the attributes of a frame by its identifier."""
         ...
     def get_keys(self) -> List[FrameIdentifier]:
-        """
-        Return a list of all ``FrameIdentifier``s described by this ``FrameSet``
-        """
+        """Return a list of all ``FrameIdentifier``s described by this ``FrameSet``."""
         ...
     def insert(self, identifier: FrameIdentifier, attributes: Dict[str, AttributeValue]):
-        """
-        Insert a new ``FrameIdentifier``, overwriting any existing one.
-        """
+        """Insert a new ``FrameIdentifier``, overwriting any existing one."""
         ...
     def merge(self, other: FrameSet):
-        """
-        Merge another ``FrameSet`` into this one, overwriting any existing keys.
-        """
+        """Merge another ``FrameSet`` into this one, overwriting any existing keys."""
     def intersection(self, identifiers: FrozenSet[FrameIdentifier]) -> "FrameSet":
-        """
-        Return a new ``FrameSet`` which describes only the given ``FrameIdentifier``s
-        """
+        """Return a new ``FrameSet`` which describes only the given ``FrameIdentifier``s."""
         ...
     def is_empty(self) -> bool:
-        """
-        Returns ``True`` if this ``FrameSet`` defines no frames.
-        """
+        """Returns ``True`` if this ``FrameSet`` defines no frames."""
         ...
     def to_instructions(self) -> List[Instruction]:
-        """
-        Return the Quil instructions which define the contained frames.
-        """
+        """Return the Quil instructions which define the contained frames."""
         ...
     def get_all_frames(self) -> Dict[FrameIdentifier, Dict[str, AttributeValue]]: ...
 
 class MemoryRegion:
     @staticmethod
     def __new__(cls, size: Vector, sharing: Optional[Sharing]) -> "MemoryRegion": ...
     @property
```

### Comparing `quil-0.9.0rc0/quil-py/quil.html` & `quil-0.9.1rc0/quil-py/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/expression.rs` & `quil-0.9.1rc0/quil-py/src/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/calibration.rs` & `quil-0.9.1rc0/quil-py/src/instruction/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/circuit.rs` & `quil-0.9.1rc0/quil-py/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/classical.rs` & `quil-0.9.1rc0/quil-py/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/control_flow.rs` & `quil-0.9.1rc0/quil-py/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/declaration.rs` & `quil-0.9.1rc0/quil-py/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/frame.rs` & `quil-0.9.1rc0/quil-py/src/instruction/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/gate.rs` & `quil-0.9.1rc0/quil-py/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/measurement.rs` & `quil-0.9.1rc0/quil-py/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/mod.rs` & `quil-0.9.1rc0/quil-py/src/instruction/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/pragma.rs` & `quil-0.9.1rc0/quil-py/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/qubit.rs` & `quil-0.9.1rc0/quil-py/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/reset.rs` & `quil-0.9.1rc0/quil-py/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/timing.rs` & `quil-0.9.1rc0/quil-py/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/instruction/waveform.rs` & `quil-0.9.1rc0/quil-py/src/instruction/waveform.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/lib.rs` & `quil-0.9.1rc0/quil-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/program/analysis.rs` & `quil-0.9.1rc0/quil-py/src/program/analysis.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-use pyo3::exceptions::PyValueError;
+use pyo3::{exceptions::PyValueError, types::PyType};
 use quil_rs::program::analysis::{
     BasicBlock, BasicBlockOwned, BasicBlockScheduleError, ControlFlowGraph, ControlFlowGraphOwned,
     QubitGraph, QubitGraphError,
 };
 use rigetti_pyo3::{
     impl_repr, py_wrap_error, py_wrap_type, pyo3::prelude::*, wrap_error, PyWrapper, ToPythonError,
 };
 
 use crate::instruction::{PyInstruction, PyTarget};
 
 use super::{scheduling::PyScheduleSeconds, PyProgram};
 
 py_wrap_type! {
+    #[pyo3(subclass)]
     PyControlFlowGraph(ControlFlowGraphOwned) as "ControlFlowGraph"
 }
 
 impl_repr!(PyControlFlowGraph);
 
 #[pymethods]
 impl PyControlFlowGraph {
+    #[new]
+    #[classmethod]
+    pub fn new(_: Py<PyType>, instance: Self) -> Self {
+        instance
+    }
+
     pub fn has_dynamic_control_flow(&self) -> bool {
         ControlFlowGraph::from(self.as_inner()).has_dynamic_control_flow()
     }
 
     pub fn basic_blocks(&self) -> Vec<PyBasicBlock> {
         ControlFlowGraph::from(self.as_inner())
             .into_blocks()
@@ -30,14 +37,15 @@
             .map(BasicBlockOwned::from)
             .map(PyBasicBlock::from)
             .collect()
     }
 }
 
 py_wrap_type! {
+    #[pyo3(subclass)]
     PyBasicBlock(BasicBlockOwned) as "BasicBlock"
 }
 impl_repr!(PyBasicBlock);
 
 wrap_error!(RustBasicBlockScheduleError(BasicBlockScheduleError));
 py_wrap_error!(
     quil,
@@ -47,14 +55,20 @@
 );
 
 wrap_error!(RustQubitGraphError(QubitGraphError));
 py_wrap_error!(quil, RustQubitGraphError, PyQubitGraphError, PyValueError);
 
 #[pymethods]
 impl PyBasicBlock {
+    #[new]
+    #[classmethod]
+    pub fn new(_: Py<PyType>, instance: Self) -> Self {
+        instance
+    }
+
     pub fn as_schedule_seconds(&self, program: &PyProgram) -> PyResult<PyScheduleSeconds> {
         BasicBlock::from(self.as_inner())
             .as_schedule_seconds(program.as_inner())
             .map(|v| v.into())
             .map_err(RustBasicBlockScheduleError::from)
             .map_err(RustBasicBlockScheduleError::to_py_err)
     }
```

### Comparing `quil-0.9.0rc0/quil-py/src/program/calibration.rs` & `quil-0.9.1rc0/quil-py/src/program/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/program/frame.rs` & `quil-0.9.1rc0/quil-py/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/program/memory.rs` & `quil-0.9.1rc0/quil-py/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/program/mod.rs` & `quil-0.9.1rc0/quil-py/src/program/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/src/validation/identifier.rs` & `quil-0.9.1rc0/quil-py/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/quil-py/test/instructions/test_copy.py` & `quil-0.9.1rc0/quil-py/test/instructions/test_copy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 from copy import copy, deepcopy
 
 from quil.expression import Expression
-from quil.instructions import Qubit, QubitPlaceholder, FrameIdentifier, Pulse, WaveformInvocation, Instruction, Calibration, Delay
+from quil.instructions import (
+    Calibration,
+    Delay,
+    FrameIdentifier,
+    Instruction,
+    Pulse,
+    Qubit,
+    QubitPlaceholder,
+    WaveformInvocation,
+)
+
 
 def test_instruction_with_qubit():
     frame_identifier = FrameIdentifier("frame", [Qubit.from_placeholder(QubitPlaceholder())])
     waveform_invocation = WaveformInvocation("wf", {})
     pulse = Pulse(False, frame_identifier, waveform_invocation)
 
     pulse_copy = copy(pulse)
@@ -14,33 +24,30 @@
     assert pulse_copy == pulse
 
     pulse_deepcopy = deepcopy(pulse)
     assert pulse_deepcopy.blocking == pulse.blocking
     assert pulse_deepcopy.waveform == pulse.waveform
     assert pulse_deepcopy.frame.name == pulse.frame.name
     assert pulse_deepcopy.frame.qubits != pulse.frame.qubits
-    
+
     instruction = Instruction(pulse)
     instruction_deepcopy = deepcopy(instruction)
     assert instruction_deepcopy != instruction
 
 
 def test_instruction_with_duplicate_placeholders():
     placeholder = Qubit.from_placeholder(QubitPlaceholder())
 
     calibration = Calibration(
-            "MYCAL",
-            [],
-            [placeholder],
-            [
-                Instruction.from_delay(
-                    Delay(Expression.from_number(complex(0.5)), [], [placeholder])
-                )
-            ],
-            [])
+        "MYCAL",
+        [],
+        [placeholder],
+        [Instruction.from_delay(Delay(Expression.from_number(complex(0.5)), [], [placeholder]))],
+        [],
+    )
 
     calibration_copy = copy(calibration)
     assert calibration_copy == calibration
 
     calibration_deepcopy = deepcopy(calibration)
     assert calibration_deepcopy != calibration
```

### Comparing `quil-0.9.0rc0/quil-py/test/program/test_program.py` & `quil-0.9.1rc0/quil-py/test/program/test_program.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pickle
-import pytest
 from typing import Optional
 
+import pytest
 from syrupy.assertion import SnapshotAssertion
 
+from quil.instructions import Gate, Instruction, Jump, Qubit, QubitPlaceholder, Target, TargetPlaceholder
 from quil.program import Program
-from quil.instructions import Instruction, QubitPlaceholder, TargetPlaceholder, Gate, Qubit, Jump, Target
 
 
 def test_pickle():
     program = Program.parse(
         """
 DECLARE ro BIT[2]
 H 0
@@ -48,61 +48,66 @@
 
     program.resolve_placeholders_with_custom_resolvers(target_resolver=target_resolver, qubit_resolver=qubit_resolver)
 
     print(program.to_quil_or_debug())
 
     assert program.to_quil() == "H 9\nJUMP @test\n"
 
+
 def test_single_block_control_flow_analysis():
     program = Program.parse(
         """
 DECLARE ro BIT[2]
 H 0
 CNOT 0 1
 MEASURE 0 ro[0]
 MEASURE 1 ro[1]
-""")
+"""
+    )
     assert program.get_used_qubits() == {Qubit.from_fixed(0), Qubit.from_fixed(1)}
     cfg = program.control_flow_graph()
     blocks = cfg.basic_blocks()
     assert len(blocks) == 1
-    assert blocks[0].terminator() == None
+    assert blocks[0].terminator() is None
     block_program = Program()
     block_program.add_instructions(blocks[0].instructions())
-    assert block_program.to_quil() == """H 0
+    assert (
+        block_program.to_quil()
+        == """H 0
 CNOT 0 1
 MEASURE 0 ro[0]
 MEASURE 1 ro[1]
 """
+    )
+
 
 def test_multi_block_control_flow_analysis():
     program = Program.parse(
         """
 DECLARE ro BIT[1]
 LABEL @start
 MEASURE 0 ro[0]
 JUMP-UNLESS @end ro[0]
 X 0
 JUMP @start
 LABEL @end
 HALT
-""")
+"""
+    )
     assert program.get_used_qubits() == {Qubit.from_fixed(0)}
     cfg = program.control_flow_graph()
 
     assert cfg.has_dynamic_control_flow()
 
     blocks = cfg.basic_blocks()
     assert len(blocks) == 3
 
-def test_basic_block_fixed_schedule():
-    """
-    Test that a simple, realistic program can be scheduled as expected.
-    """
 
+def test_basic_block_fixed_schedule():
+    """Test that a simple, realistic program can be scheduled as expected."""
     program = Program.parse(
         """DEFFRAME 0 "flux_tx_cz":
     TEST: 1
 
 DEFFRAME 1 "flux_tx_iswap":
     TEST: 1
 
@@ -134,39 +139,41 @@
     SHIFT-PHASE q0 "flux_tx_cz" 1.0
     SHIFT-PHASE q1 "flux_tx_iswap" 1.0
     FENCE q0 q1
 
 CZ 0 1
 CZ 2 3
 CZ 0 2
-""")
+"""
+    )
     cfg = program.control_flow_graph()
     blocks = cfg.basic_blocks()
     assert len(blocks) == 1
     block = blocks[0]
 
     schedule = block.as_schedule_seconds(program)
     items = schedule.items()
 
     # One for each CZ
     assert len(items) == 3
 
-    items = { item.instruction_index: item for item in items }
+    items = {item.instruction_index: item for item in items}
 
     # The first CZ should start at 0
     assert items[0].time_span.start == 0.0
 
     # The first CZ should start and end at the same times
     assert items[0].time_span.start == items[1].time_span.start
     assert items[0].time_span.duration == items[1].time_span.duration
 
     # The third CZ should start when the first and second ones end and be of the same duration
     assert items[0].time_span.start + items[0].time_span.duration == items[2].time_span.start
     assert items[0].time_span.duration == items[2].time_span.duration
 
+
 def test_filter_instructions(snapshot: SnapshotAssertion):
     input = """DECLARE foo REAL[1]
 DEFFRAME 1 "rx":
 \tHARDWARE-OBJECT: "hardware"
 DEFCAL I 1:
 \tDELAY 0 1
 DEFGATE BAR AS MATRIX:
```

### Comparing `quil-0.9.0rc0/quil-py/test/test_eq.py` & `quil-0.9.1rc0/quil-py/test/test_eq.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from copy import deepcopy
 
 import numpy as np
 
-from quil.instructions import Instruction, Gate, Qubit
 from quil.expression import Expression
+from quil.instructions import Gate, Instruction, Qubit
 from quil.program import Program
 
+
 def test_instruction_eq():
     pi_expr = Expression.from_number(complex(np.pi, 0))
 
     rx = Gate("RX", [pi_expr], [Qubit.from_fixed(0)], [])
     rx_copy = deepcopy(rx)
     ry = Gate("RY", [pi_expr], [Qubit.from_fixed(0)], [])
     assert rx == rx_copy
@@ -21,14 +22,15 @@
     rx_inst_copy = deepcopy(rx_inst)
     ry_inst = Instruction.from_gate(ry)
     assert rx_inst == rx_inst_copy
     assert not (rx_inst != rx_inst_copy)
     assert rx_inst != ry_inst
     assert not (rx_inst == ry_inst)
 
+
 def test_program_eq():
     p1 = Program.parse("DECLARE ro BIT\nRX(pi) 0")
     p1_copy = deepcopy(p1)
     p2 = Program.parse("DECLARE theta BIT\nRX(pi) 0")
 
     assert p1 == p1_copy
     assert not (p1 != p1_copy)
```

### Comparing `quil-0.9.0rc0/Cargo.lock` & `quil-0.9.1rc0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1082,38 +1082,38 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quil-cli"
-version = "0.2.0-rc.1"
+version = "0.2.1-rc.0"
 dependencies = [
  "anyhow",
  "clap",
  "quil-rs",
 ]
 
 [[package]]
 name = "quil-py"
-version = "0.9.0-rc.0"
+version = "0.9.1-rc.0"
 dependencies = [
  "indexmap",
  "ndarray",
  "numpy",
  "pyo3",
  "pyo3-build-config",
  "quil-rs",
  "rigetti-pyo3",
  "strum",
 ]
 
 [[package]]
 name = "quil-rs"
-version = "0.25.0-rc.0"
+version = "0.25.1-rc.0"
 dependencies = [
  "approx",
  "clap",
  "criterion",
  "dot-writer",
  "indexmap",
  "insta",
```

### Comparing `quil-0.9.0rc0/quil/program/__init__.pyi` & `quil-0.9.1rc0/quil/program/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from typing import Dict, FrozenSet, Set, final, List, Optional, Sequence, Callable
+from typing import Callable, Dict, FrozenSet, List, Optional, Sequence, Set, final
 
 import numpy as np
 from numpy.typing import NDArray
+from typing_extensions import Self
+
 from quil.instructions import (
     AttributeValue,
     Calibration,
     Declaration,
     FrameIdentifier,
     Gate,
     GateDefinition,
     Instruction,
     MeasureCalibrationDefinition,
     Measurement,
     MemoryReference,
     Qubit,
+    QubitPlaceholder,
     Sharing,
     Target,
+    TargetPlaceholder,
     Vector,
     Waveform,
-    TargetPlaceholder,
-    QubitPlaceholder,
 )
 
 @final
 class Program:
     @staticmethod
     def __new__(cls) -> "Program": ...
     @property
@@ -47,95 +49,78 @@
     @property
     def memory_regions(self) -> Dict[str, MemoryRegion]: ...
     @memory_regions.setter
     def memory_regions(self, memory_regions: Dict[str, MemoryRegion]): ...
     @property
     def declarations(self) -> Dict[str, Declaration]: ...
     def dagger(self) -> "Program":
-        """
-        Creates a new conjugate transpose of the ``Program`` by reversing the order of gate
-        instructions and applying the DAGGER modifier to each.
+        """Creates a new conjugate transpose of the ``Program`` by reversing the order of gate instructions and applying the DAGGER modifier to each.
 
         Raises a ``GateError`` if any of the instructions in the program are not a ``Gate`
         """
         ...
     def expand_calibrations(self) -> "Program":
-        """
-        Expand any instructions in the program which have a matching calibration, leaving the others
-        unchanged. Recurses though each instruction while ensuring there is no cycle in the expansion
-        graph (i.e. no calibration expands directly or indirectly into itself)
+        """Expand any instructions in the program which have a matching calibration, leaving the others unchanged.
+
+        Recurses though each instruction while ensuring there is no cycle in the expansion graph (i.e. no calibration
+        expands directly or indirectly into itself)
         """
         ...
     def into_simplified(self) -> "Program":
-        """
-        Simplify this program into a new [`Program`] which contains only instructions
-        and definitions which are executed; effectively, perform dead code removal.
+        """Simplify this program into a new `Program` which contains only instructions and definitions which are executed; effectively, perform dead code removal.
 
         Removes:
         - All calibrations, following calibration expansion
         - Frame definitions which are not used by any instruction such as `PULSE` or `CAPTURE`
         - Waveform definitions which are not used by any instruction
 
         When a valid program is simplified, it remains valid.
         """
         ...
     def get_used_qubits(self) -> Set[Qubit]:
-        """
-        Returns a set consisting of every Qubit that is used in the program.
-        """
+        """Returns a set consisting of every Qubit that is used in the program."""
         ...
     def add_instruction(self, instruction: Instruction):
-        """
-        Add an instruction to the end of the program.
-        """
+        """Add an instruction to the end of the program."""
         ...
     def add_instructions(self, instructions: Sequence[Instruction]):
-        """
-        Add a list of instructions to the end of the program.
-        """
+        """Add a list of instructions to the end of the program."""
         ...
     @staticmethod
     def parse(input: str) -> "Program":
-        """
-        Parses the given Quil string and returns a new ``Program``.
+        """Parses the given Quil string and returns a new ``Program``.
+
         Raises a ``ProgramError`` if the given string isn't valid Quil.
         """
     def to_instructions(self) -> Sequence[Instruction]: ...
     def to_unitary(self, n_qubits: int) -> NDArray[np.complex_]: ...
     def copy(self) -> "Program":
-        """
-        Creates a clone of this ``Program``.
-        """
+        """Creates a clone of this ``Program``."""
         ...
     def clone_without_body_instructions(self) -> "Program":
-        """
-        Creates a clone of this ``Program`` with an empty body instructions list.
-        """
+        """Creates a clone of this ``Program`` with an empty body instructions list."""
     def __add__(self, rhs: Program) -> Program: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def filter_instructions(self, predicate: Callable[[Instruction], bool]) -> "Program":
-        """
-        Return a new ``Program`` containing only the instructions for which ``predicate`` returns ``True``.
-        """
+        """Return a new ``Program`` containing only the instructions for which ``predicate`` returns ``True``."""
         ...
     def wrap_in_loop(
         self, loop_count_reference: MemoryReference, start_target: Target, end_target: Target, iterations: int
     ) -> "Program":
-        """
-        Return a copy of the `Program` wrapped in a loop that repeats ``iterations`` times.
+        """Return a copy of the `Program` wrapped in a loop that repeats ``iterations`` times.
 
         The loop is constructed by wrapping the body of the program in classical Quil instructions.
         The given ``loop_count_reference`` must refer to an INTEGER memory region. The value at the
         reference given will be set to ``iterations`` and decremented in the loop. The loop will
         terminate when the reference reaches 0. For this reason your program should not itself
         modify the value at the reference unless you intend to modify the remaining number of
         iterations (i.e. to break the loop).
@@ -145,54 +130,51 @@
         used elsewhere in the program.
 
         If `iterations` is 0, then a copy of the program is returned without any changes. Raises a
         `TypeError` if `iterations` is negative.
         """
         ...
     def resolve_placeholders(self) -> None:
-        """
-        Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program using default resolvers.
+        """Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program using default resolvers.
 
         The default resolver will be used to generate a unique value for that placeholder within the scope of
         the program using an auto-incrementing value (for qubit) or suffix (for target)
         while ensuring that unique value is not already in use within the program.
         """
         ...
     def resolve_placeholders_with_custom_resolvers(
         self,
         *,
         target_resolver: Optional[Callable[[TargetPlaceholder], Optional[str]]] = None,
         qubit_resolver: Optional[Callable[[QubitPlaceholder], Optional[int]]] = None,
     ):
-        """
-        Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program such that the resolved values
-        will remain unique to that placeholder within the scope of the program.
+        """Resolve ``TargetPlaceholder``s and ``QubitPlaceholder``s within the program.
+
+        The resolved values will remain unique to that placeholder within the scope of the program.
 
         If you provide ``target_resolver`` and/or ``qubit_resolver``, those will be used to resolve those values respectively.
         If your resolver returns `None` for a particular placeholder, it will not be replaced but will be left as a placeholder.
 
         If you do not provide a resolver for a placeholder, a default resolver will be used which will generate a unique value
         for that placeholder within the scope of the program using an auto-incrementing value (for qubit) or suffix (for target)
         while ensuring that unique value is not already in use within the program.
         """
         ...
     def control_flow_graph(self) -> "ControlFlowGraph":
-        """
-        Return the `control flow graph`_ of the program.
+        """Return the `control flow graph`_ of the program.
 
         .. _control flow graph: https://en.wikipedia.org/wiki/Control-flow_graph
         """
 
-@final
 class BasicBlock:
-    def as_schedule_seconds(self, program: Program) -> ScheduleSeconds:
-        """
-        Return the ``ScheduleSeconds`` representing the timing of the instructions within the block.
+    def __new__(cls, instance: "BasicBlock") -> Self:
+        """Create a new instance of a `BasicBlock` (or a subclass) using an existing instance."""
 
-        This schedule is computed by:
+    def as_schedule_seconds(self, program: Program) -> ScheduleSeconds:
+        """Return the ``ScheduleSeconds`` representing the timing of the instructions within the block.
 
         * Expanding each instruction within the block using the program's calibration definitions
         * Resolving the `ScheduleSeconds` of the expanded instructions
         * Mapping calibrated instructions back to the original instructions within this block, such that the
           block's instruction is represented as a timespan encompassing all of its expanded instructions
 
         Note: the schedule will not include instructions with zero duration (such as `FENCE`).
@@ -253,33 +235,27 @@
                 A 0
                 B 0 1
 
         `B 0` will be scheduled from time 0 to time 2, because its inner `FENCE` is scheduled for time 0.
         This may be unexpected if the user expects to see only the timing of the inner `PULSE`.
         """
     def gate_depth(self, gate_minimum_qubit_count: int) -> int:
-        """
-        Returns the length of the longest path from an initial instruction (one with no prerequisite instructions) to a final
-        instruction (one with no dependent instructions), where the length of a path is the number of gate instructions in the path.
+        """Returns the length of the longest path from an initial instruction (one with no prerequisite instructions) to a final instruction (one with no dependent instructions), where the length of a path is the number of gate instructions in the path.
 
         :param gate_minimum_qubit_count: The minimum number of qubits in a gate for it to be counted in the depth.
         """
     def label(self) -> Optional[Target]:
-        """
-        Return the label of the block, if any. This is used to target this block in control flow.
-        """
+        """Return the label of the block, if any. This is used to target this block in control flow."""
     def instructions(self) -> List[Instruction]:
-        """
-        Return a list of the instructions in the block, in order of definition.
+        """Return a list of the instructions in the block, in order of definition.
 
         This does not include the label or terminator instructions.
         """
     def terminator(self) -> Optional[Instruction]:
-        """
-        Return the control flow terminator instruction of the block, if any.
+        """Return the control flow terminator instruction of the block, if any.
 
         If this is ``None``, the implicit behavior is to "continue" to the subsequent block.
         """
 
 @final
 class CalibrationSet:
     @staticmethod
@@ -289,184 +265,141 @@
         measure_calibration_definitions: Sequence[MeasureCalibrationDefinition],
     ) -> "CalibrationSet": ...
     @property
     def calibrations(self) -> List[Calibration]: ...
     @property
     def measure_calibrations(self) -> List[MeasureCalibrationDefinition]: ...
     def expand(self, instruction: Instruction, previous_calibrations: Sequence[Instruction]) -> List[Instruction]:
-        """
-        Given an instruction, return the instructions to which it is expanded if there is a match.
+        """Given an instruction, return the instructions to which it is expanded if there is a match.
+
         Recursively calibrate instructions, returning an error if a calibration directly or indirectly
         expands into itself.
         """
     ...
 
     def get_match_for_measurement(self, measurement: Measurement) -> Optional[MeasureCalibrationDefinition]:
-        """
-        Returns the last-specified ``MeasureCalibrationDefinition`` that matches the target
-        qubit (if any), or otherwise the last-specified one that specified no qubit.
-        """
+        """Returns the last-specified ``MeasureCalibrationDefinition`` that matches the target qubit (if any), or otherwise the last-specified one that specified no qubit."""
         ...
     def get_match_for_gate(self, gate: Gate) -> Optional[Calibration]:
-        """
-        Return the final calibration which matches the gate per the QuilT specification:
+        """Return the final calibration which matches the gate per the QuilT specification.
 
         A calibration matches a gate if:
         1. It has the same name
         2. It has the same modifiers
         3. It has the same qubit count (any mix of fixed & variable)
         4. It has the same parameter count (both specified and unspecified)
         5. All fixed qubits in the calibration definition match those in the gate
         6. All specified parameters in the calibration definition match those in the gate
         """
     def __len__(self) -> int: ...
     def is_empty(self) -> bool:
         """Returns ``True`` if the ``CalibrationSet`` contains no data."""
         ...
     def insert_calibration(self, calibration: Calibration) -> Optional[Calibration]:
-        """
-        Insert another ``Calibration`` (`DEFCAL`) to the set.
+        """Insert another ``Calibration`` (`DEFCAL`) to the set.
 
         If a calibration with the same name already exists, it is overwritten and this
         function returns the previous calibration. Otherwise, None is returned.
         """
         ...
-    def insert_measurement_calibration(self, calibration: MeasureCalibrationDefinition) -> Optional[MeasureCalibrationDefinition]:
-        """
-        Add another ``MeasureCalibrationDefinition`` (`DEFCAL MEASURE`) to the set
+    def insert_measurement_calibration(
+        self, calibration: MeasureCalibrationDefinition
+    ) -> Optional[MeasureCalibrationDefinition]:
+        """Add another ``MeasureCalibrationDefinition`` (`DEFCAL MEASURE`) to the set.
 
         If a calibration with the same name already exists, it is overwritten and this
         function returns the previous calibration. Otherwise, None is returned.
         """
     def extend(self, other: CalibrationSet):
-        """
-        Append another [`CalibrationSet`] onto this one
-        """
+        """Append another [`CalibrationSet`] onto this one."""
         ...
     def to_instructions(self):
-        """
-        Return the Quil instructions which describe the contained calibrations
-        """
+        """Return the Quil instructions which describe the contained calibrations."""
         ...
 
-
-@final
 class ScheduleSecondsItem:
-    """
-    A single item within a fixed schedule, representing a single instruction within a basic block.
-    """
+    """A single item within a fixed schedule, representing a single instruction within a basic block."""
+
     @property
     def instruction_index(self) -> int:
-        """
-        The index of the instruction within the basic block.
-        """
+        """The index of the instruction within the basic block."""
     @property
     def time_span(self) -> TimeSpanSeconds:
-        """
-        The time span during which the instruction is scheduled.
-        """
-
+        """The time span during which the instruction is scheduled."""
 
-@final
 class ControlFlowGraph:
-    """
-    Representation of a control flow graph (CFG) for a Quil program.
+    """Representation of a control flow graph (CFG) for a Quil program.
 
     The CFG is a directed graph where each node is a basic block and each edge is a control flow
     transition between two basic blocks.
     """
+    def __new__(cls, instance: "ControlFlowGraph") -> Self:
+        """Create a new instance of a `ControlFlowGraph` (or a subclass) using an existing instance."""
 
-    def has_dynamic_control_flow(self) -> bool: 
-        """
-        Return ``True`` if the program has dynamic control flow, i.e. contains a conditional branch instruction.
+    def has_dynamic_control_flow(self) -> bool:
+        """Return ``True`` if the program has dynamic control flow, i.e. contains a conditional branch instruction.
 
         ``False`` does not imply that there is only one basic block in the program. Multiple basic blocks may have
         non-conditional control flow among them, in which the execution order is deterministic and does not depend
         on program state. This may be a sequence of basic blocks with fixed `JUMP`s or without explicit terminators.
         """
-    def basic_blocks(self) -> List["BasicBlock"]: 
-        """
-        Return a list of all the basic blocks in the control flow graph, in order of definition.
-        """
+    def basic_blocks(self) -> List["BasicBlock"]:
+        """Return a list of all the basic blocks in the control flow graph, in order of definition."""
 
-@final
 class ScheduleSeconds:
     def items(self) -> List[ScheduleSecondsItem]:
-        """
-        All the items in the schedule, in unspecified order.
-        """
+        """All the items in the schedule, in unspecified order."""
     def duration(self) -> float:
-        """
-        The duration of the schedule, in seconds.
+        """The duration of the schedule, in seconds.
 
         This is the maximum of the end time of all the items.
         """
 
-@final
 class TimeSpanSeconds:
-    """
-    Representation of a time span in seconds.
-    """
+    """Representation of a time span in seconds."""
+
     @property
     def start(self) -> float:
-        """
-        The start time of the time span, in seconds.
+        """The start time of the time span, in seconds.
 
         This is relative to the start of the scheduling context (such as the basic block).
         """
     @property
     def duration(self) -> float:
-        """
-        The duration of the time span, in seconds.
-        """
+        """The duration of the time span, in seconds."""
     @property
     def end(self) -> float:
-        """
-        The end time of the time span, in seconds.
+        """The end time of the time span, in seconds.
 
         This is the sum of the start time and duration.
         """
 
 @final
 class FrameSet:
     @staticmethod
     def __new__(cls) -> "FrameSet": ...
     def get(self, identifier: FrameIdentifier) -> Optional[Dict[str, AttributeValue]]:
-        """
-        Retrieve the attributes of a frame by its identifier
-        """
+        """Retrieve the attributes of a frame by its identifier."""
         ...
     def get_keys(self) -> List[FrameIdentifier]:
-        """
-        Return a list of all ``FrameIdentifier``s described by this ``FrameSet``
-        """
+        """Return a list of all ``FrameIdentifier``s described by this ``FrameSet``."""
         ...
     def insert(self, identifier: FrameIdentifier, attributes: Dict[str, AttributeValue]):
-        """
-        Insert a new ``FrameIdentifier``, overwriting any existing one.
-        """
+        """Insert a new ``FrameIdentifier``, overwriting any existing one."""
         ...
     def merge(self, other: FrameSet):
-        """
-        Merge another ``FrameSet`` into this one, overwriting any existing keys.
-        """
+        """Merge another ``FrameSet`` into this one, overwriting any existing keys."""
     def intersection(self, identifiers: FrozenSet[FrameIdentifier]) -> "FrameSet":
-        """
-        Return a new ``FrameSet`` which describes only the given ``FrameIdentifier``s
-        """
+        """Return a new ``FrameSet`` which describes only the given ``FrameIdentifier``s."""
         ...
     def is_empty(self) -> bool:
-        """
-        Returns ``True`` if this ``FrameSet`` defines no frames.
-        """
+        """Returns ``True`` if this ``FrameSet`` defines no frames."""
         ...
     def to_instructions(self) -> List[Instruction]:
-        """
-        Return the Quil instructions which define the contained frames.
-        """
+        """Return the Quil instructions which define the contained frames."""
         ...
     def get_all_frames(self) -> Dict[FrameIdentifier, Dict[str, AttributeValue]]: ...
 
 class MemoryRegion:
     @staticmethod
     def __new__(cls, size: Vector, sharing: Optional[Sharing]) -> "MemoryRegion": ...
     @property
```

### Comparing `quil-0.9.0rc0/quil/instructions/__init__.pyi` & `quil-0.9.1rc0/quil/instructions/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from enum import Enum
+from typing import Dict, List, Optional, Sequence, Tuple, Union, final
+
 import numpy as np
 from numpy.typing import NDArray
-from typing import Dict, List, Optional, Sequence, Tuple, Union, final
 from typing_extensions import Self
 
 from quil.expression import Expression
 
 @final
 class Instruction:
-    """
-    A Quil instruction. Each variant corresponds to a possible type of Quil instruction.
+    """A Quil instruction. Each variant corresponds to a possible type of Quil instruction.
 
     # Variants:
     - ``arithmetic``: An arithmetic expression defined by an ``Arithmetic``.
     - ``binary_logic``: A binary expression defined by a ``BinaryLogic``.
     - ``calibration_definition``: Corresponds to a `DEFCAL` instruction (not `DEFCAL MEASURE`)
     -     defined by a ``Calibration``.
     - ``capture``: Corresponds to a `CAPTURE` instruction
@@ -109,21 +109,17 @@
             ShiftPhase,
             Store,
             SwapPhases,
             UnaryLogic,
             WaveformDefinition,
         ],
     ) -> Self:
-        """
-        Returns a new ``Instruction`` from the given inner data.
-        """
+        """Returns a new ``Instruction`` from the given inner data."""
     def is_quil_t(self) -> bool:
-        """
-        Returns ``True`` if the instruction is a Quil-T instruction, ``False`` otherwise.
-        """
+        """Returns ``True`` if the instruction is a Quil-T instruction, ``False`` otherwise."""
         ...
     def inner(
         self,
     ) -> Union[
         Arithmetic,
         Calibration,
         Capture,
@@ -157,17 +153,15 @@
         ShiftFrequency,
         ShiftPhase,
         Store,
         SwapPhases,
         UnaryLogic,
         WaveformDefinition,
     ]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_arithmetic(self) -> bool: ...
     def is_binary_logic(self) -> bool: ...
     def is_calibration_definition(self) -> bool: ...
     def is_capture(self) -> bool: ...
     def is_circuit_definition(self) -> bool: ...
     def is_convert(self) -> bool: ...
@@ -201,99 +195,99 @@
     def is_shift_phase(self) -> bool: ...
     def is_unary_logic(self) -> bool: ...
     def is_store(self) -> bool: ...
     def is_swap_phases(self) -> bool: ...
     def is_waveform_definition(self) -> bool: ...
     def is_wait(self) -> bool: ...
     @staticmethod
-    def new_halt() -> "Instruction": ...
+    def new_halt() -> Instruction: ...
     @staticmethod
-    def new_nop() -> "Instruction": ...
+    def new_nop() -> Instruction: ...
     @staticmethod
-    def new_wait() -> "Instruction": ...
+    def new_wait() -> Instruction: ...
     @staticmethod
-    def from_arithmetic(inner: Arithmetic) -> "Instruction": ...
+    def from_arithmetic(inner: Arithmetic) -> Instruction: ...
     @staticmethod
-    def from_binary_logic(inner: BinaryLogic) -> "Instruction": ...
+    def from_binary_logic(inner: BinaryLogic) -> Instruction: ...
     @staticmethod
-    def from_calibration_definition(inner: Calibration) -> "Instruction": ...
+    def from_calibration_definition(inner: Calibration) -> Instruction: ...
     @staticmethod
-    def from_capture(inner: Capture) -> "Instruction": ...
+    def from_capture(inner: Capture) -> Instruction: ...
     @staticmethod
     def from_circuit_definition(
         inner: CircuitDefinition,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     @staticmethod
-    def from_convert(inner: Convert) -> "Instruction": ...
+    def from_convert(inner: Convert) -> Instruction: ...
     @staticmethod
-    def from_comparison(inner: Comparison) -> "Instruction": ...
+    def from_comparison(inner: Comparison) -> Instruction: ...
     @staticmethod
-    def from_declaration(inner: Declaration) -> "Instruction": ...
+    def from_declaration(inner: Declaration) -> Instruction: ...
     @staticmethod
-    def from_delay(inner: Delay) -> "Instruction": ...
+    def from_delay(inner: Delay) -> Instruction: ...
     @staticmethod
-    def from_exchange(inner: Exchange) -> "Instruction": ...
+    def from_exchange(inner: Exchange) -> Instruction: ...
     @staticmethod
-    def from_fence(inner: Fence) -> "Instruction": ...
+    def from_fence(inner: Fence) -> Instruction: ...
     @staticmethod
-    def from_frame_definition(inner: FrameDefinition) -> "Instruction": ...
+    def from_frame_definition(inner: FrameDefinition) -> Instruction: ...
     @staticmethod
-    def from_gate(inner: Gate) -> "Instruction": ...
+    def from_gate(inner: Gate) -> Instruction: ...
     @staticmethod
-    def from_gate_definition(inner: GateDefinition) -> "Instruction": ...
+    def from_gate_definition(inner: GateDefinition) -> Instruction: ...
     @staticmethod
-    def from_include(inner: Include) -> "Instruction": ...
+    def from_include(inner: Include) -> Instruction: ...
     @staticmethod
-    def from_jump(inner: Jump) -> "Instruction": ...
+    def from_jump(inner: Jump) -> Instruction: ...
     @staticmethod
-    def from_jump_when(inner: JumpWhen) -> "Instruction": ...
+    def from_jump_when(inner: JumpWhen) -> Instruction: ...
     @staticmethod
-    def from_jump_unless(inner: JumpUnless) -> "Instruction": ...
+    def from_jump_unless(inner: JumpUnless) -> Instruction: ...
     @staticmethod
-    def from_label(inner: Label) -> "Instruction": ...
+    def from_label(inner: Label) -> Instruction: ...
     @staticmethod
-    def from_load(inner: Load) -> "Instruction": ...
+    def from_load(inner: Load) -> Instruction: ...
     @staticmethod
     def from_measure_calibration_definition(
         inner: MeasureCalibrationDefinition,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     @staticmethod
     def from_measurement(
         inner: Measurement,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     @staticmethod
-    def from_move(inner: Move) -> "Instruction": ...
+    def from_move(inner: Move) -> Instruction: ...
     @staticmethod
-    def from_pragma(inner: Pragma) -> "Instruction": ...
+    def from_pragma(inner: Pragma) -> Instruction: ...
     @staticmethod
-    def from_pulse(inner: Pulse) -> "Instruction": ...
+    def from_pulse(inner: Pulse) -> Instruction: ...
     @staticmethod
-    def from_raw_capture(inner: RawCapture) -> "Instruction": ...
+    def from_raw_capture(inner: RawCapture) -> Instruction: ...
     @staticmethod
-    def from_set_frequency(inner: SetFrequency) -> "Instruction": ...
+    def from_set_frequency(inner: SetFrequency) -> Instruction: ...
     @staticmethod
-    def from_set_phase(inner: SetPhase) -> "Instruction": ...
+    def from_set_phase(inner: SetPhase) -> Instruction: ...
     @staticmethod
-    def from_set_scale(inner: SetScale) -> "Instruction": ...
+    def from_set_scale(inner: SetScale) -> Instruction: ...
     @staticmethod
-    def from_shift_frequency(inner: ShiftFrequency) -> "Instruction": ...
+    def from_shift_frequency(inner: ShiftFrequency) -> Instruction: ...
     @staticmethod
-    def from_shift_phase(inner: ShiftPhase) -> "Instruction": ...
+    def from_shift_phase(inner: ShiftPhase) -> Instruction: ...
     @staticmethod
-    def from_unary_logic(inner: UnaryLogic) -> "Instruction": ...
+    def from_unary_logic(inner: UnaryLogic) -> Instruction: ...
     @staticmethod
-    def from_store(inner: Store) -> "Instruction": ...
+    def from_store(inner: Store) -> Instruction: ...
     @staticmethod
-    def from_swap_phases(inner: SwapPhases) -> "Instruction": ...
+    def from_swap_phases(inner: SwapPhases) -> Instruction: ...
     @staticmethod
-    def from_reset(inner: Reset) -> "Instruction": ...
+    def from_reset(inner: Reset) -> Instruction: ...
     @staticmethod
     def from_waveform_definition(
         inner: WaveformDefinition,
-    ) -> "Instruction": ...
+    ) -> Instruction: ...
     def as_arithmetic(self) -> Optional[Arithmetic]: ...
     def to_arithmetic(self) -> Arithmetic: ...
     def as_binary_logic(self) -> Optional[BinaryLogic]: ...
     def to_binary_logic(self) -> BinaryLogic: ...
     def as_convert(self) -> Optional[Convert]: ...
     def to_convert(self) -> Convert: ...
     def as_comparison(self) -> Optional[Comparison]: ...
@@ -363,96 +357,95 @@
     def as_store(self) -> Optional[Store]: ...
     def to_store(self) -> Store: ...
     def as_swap_phases(self) -> Optional[SwapPhases]: ...
     def to_swap_phases(self) -> SwapPhases: ...
     def as_waveform_definition(self) -> Optional[WaveformDefinition]: ...
     def to_waveform_definition(self) -> WaveformDefinition: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
+        """Attempt to convert the instruction to a valid Quil string. Raises an exception if the instruction can't be converted to valid Quil."""
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class ArithmeticOperand:
-    """
-    A Quil arithmetic operand.
+    """A Quil arithmetic operand.
 
     # Variants:
     - ``literal_integer``: An integer literal.
     - ``literal_real``: A real numbered literal.
     - ``memory_reference``: A Quil ``MemoryReference``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the operand is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``ArithmeticOperand`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[int, float, MemoryReference]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_literal_integer(self) -> bool: ...
     def is_literal_real(self) -> bool: ...
     def is_memory_reference(self) -> bool: ...
     def as_literal_integer(self) -> Optional[int]: ...
     def as_literal_real(self) -> Optional[float]: ...
     def as_memory_reference(self) -> Optional[MemoryReference]: ...
     def to_literal_integer(self) -> int: ...
     def to_literal_real(self) -> float: ...
     def to_memory_reference(self) -> MemoryReference: ...
     @staticmethod
-    def from_literal_integer(inner: int) -> "ArithmeticOperand": ...
+    def from_literal_integer(inner: int) -> ArithmeticOperand: ...
     @staticmethod
-    def from_literal_real(inner: float) -> "ArithmeticOperand": ...
+    def from_literal_real(inner: float) -> ArithmeticOperand: ...
     @staticmethod
     def from_memory_reference(
         inner: MemoryReference,
-    ) -> "ArithmeticOperand": ...
+    ) -> ArithmeticOperand: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class ArithmeticOperator(Enum):
     Add = "Add"
     Subtract = "Subtract"
     Divide = "Divide"
     Multiply = "Multiply"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Arithmetic:
     def __new__(
         cls,
         operator: ArithmeticOperator,
         destination: ArithmeticOperand,
@@ -467,89 +460,88 @@
     @destination.setter
     def destination(self, operand: ArithmeticOperand) -> None: ...
     @property
     def source(self) -> ArithmeticOperand: ...
     @source.setter
     def source(self, operand: ArithmeticOperand) -> None: ...
     def to_quil(self) -> str:
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
-        ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original. Should be used by passing
+        an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class BinaryOperand:
-    """
-    A Quil binary operand.
+    """A Quil binary operand.
 
     # Variants:
     - ``literal_integer``: An integer literal.
     - ``memory_reference``: A Quil ``MemoryReference``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the operand is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``BinaryOperand`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[int, MemoryReference]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_literal_integer(self) -> bool: ...
     def is_memory_reference(self) -> bool: ...
     def as_literal_integer(self) -> Optional[int]: ...
     def as_memory_reference(self) -> Optional[MemoryReference]: ...
     def to_literal_integer(self) -> int: ...
     def to_memory_reference(self) -> MemoryReference: ...
     @staticmethod
-    def from_literal_integer(inner: int) -> "BinaryOperand": ...
+    def from_literal_integer(inner: int) -> BinaryOperand: ...
     @staticmethod
     def from_memory_reference(
         inner: MemoryReference,
-    ) -> "BinaryOperand": ...
+    ) -> BinaryOperand: ...
     def to_quil(self) -> str:
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
-        ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class BinaryOperator(Enum):
     And = "AND"
     Ior = "IOR"
     Xor = "XOR"
     def to_quil(self) -> str:
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
-        ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class BinaryOperands:
     def __new__(
         cls,
         memory_reference: MemoryReference,
         operand: BinaryOperand,
@@ -574,156 +566,173 @@
     @operator.setter
     def operator(self, operator: BinaryOperator) -> None: ...
     @property
     def operands(self) -> BinaryOperands: ...
     @operands.setter
     def operands(self, operands: BinaryOperands) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Convert:
     def __new__(cls, destination: MemoryReference, source: MemoryReference) -> Self: ...
     @property
     def destination(self) -> MemoryReference: ...
     @destination.setter
     def destination(self, destination: MemoryReference) -> None: ...
     @property
     def source(self) -> MemoryReference: ...
     @source.setter
     def source(self, source: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Move:
     def __new__(cls, destination: MemoryReference, source: ArithmeticOperand) -> Self: ...
     @property
     def destination(self) -> MemoryReference: ...
     @destination.setter
     def destination(self, destination: MemoryReference) -> None: ...
     @property
     def source(self) -> ArithmeticOperand: ...
     @source.setter
     def source(self, source: ArithmeticOperand) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Exchange:
     def __new__(cls, left: MemoryReference, right: MemoryReference) -> Self: ...
     @property
     def left(self) -> MemoryReference: ...
     @left.setter
     def left(self, left: MemoryReference) -> None: ...
     @property
     def right(self) -> MemoryReference: ...
     @right.setter
     def right(self, right: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class ComparisonOperand:
-    """
-    A Quil binary operand.
+    """A Quil binary operand.
 
     # Variants:
     - ``literal_integer``: An integer literal.
     - ``literal_real``: A floating point literal.
     - ``memory_reference``: A Quil ``MemoryReference``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the operand is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``BinaryOperand`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[int, float, MemoryReference]:
-        """
-        Returns the inner value of the variant.
-        """
+        """Returns the inner value of the variant."""
         ...
     def is_literal_integer(self) -> bool: ...
     def is_literal_real(self) -> bool: ...
     def is_memory_reference(self) -> bool: ...
     def as_literal_integer(self) -> Optional[int]: ...
     def as_literal_real(self) -> Optional[float]: ...
     def as_memory_reference(self) -> Optional[MemoryReference]: ...
     def to_literal_integer(self) -> int: ...
     def to_literal_real(self) -> float: ...
     def to_memory_reference(self) -> MemoryReference: ...
     @staticmethod
-    def from_literal_integer(inner: int) -> "ComparisonOperand": ...
+    def from_literal_integer(inner: int) -> ComparisonOperand: ...
     @staticmethod
-    def from_literal_real(inner: float) -> "ComparisonOperand": ...
+    def from_literal_real(inner: float) -> ComparisonOperand: ...
     @staticmethod
     def from_memory_reference(
         inner: MemoryReference,
-    ) -> "ComparisonOperand": ...
+    ) -> ComparisonOperand: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class ComparisonOperator(Enum):
     Equal = "EQUAL"
     GreaterThanOrEqual = "GREATERTHANOREQUAL"
     GreaterThan = "GREATERTHAN"
@@ -743,68 +752,78 @@
     @property
     def operands(
         self,
     ) -> Tuple[MemoryReference, MemoryReference, ComparisonOperand]: ...
     @operands.setter
     def operands(self, operands: Tuple[MemoryReference, MemoryReference, ComparisonOperand]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class UnaryOperator(Enum):
     Neg = "NEG"
     Not = "NOT"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class UnaryLogic:
     def __new__(cls, operator: UnaryOperator, operand: MemoryReference) -> Self: ...
     @property
     def operator(self) -> UnaryOperator: ...
     @operator.setter
     def operator(self, operator: UnaryOperator) -> None: ...
     @property
     def operand(self) -> MemoryReference: ...
     @operand.setter
     def operand(self, operand: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Calibration:
     def __new__(
         cls,
         name: str,
@@ -830,26 +849,31 @@
     @instructions.setter
     def instructions(self, instructions: Sequence[Instruction]) -> None: ...
     @property
     def modifiers(self) -> List[GateModifier]: ...
     @modifiers.setter
     def modifiers(self, modifiers: Sequence[GateModifier]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class MeasureCalibrationDefinition:
     def __new__(
         cls,
         qubit: Optional[Qubit],
@@ -865,26 +889,31 @@
     @parameter.setter
     def parameter(self, parameter: str) -> None: ...
     @property
     def instructions(self) -> List[Instruction]: ...
     @instructions.setter
     def instructions(self, instructions: Sequence[Instruction]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class CircuitDefinition:
     def __new__(
         cls,
         name: str,
@@ -905,26 +934,31 @@
     @qubit_variables.setter
     def qubit_variables(self, qubit_variables: Sequence[str]) -> None: ...
     @property
     def instructions(self) -> List[Instruction]: ...
     @instructions.setter
     def instructions(self, instructions: Sequence[Instruction]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Offset:
     def __new__(
         cls,
         offset: int,
@@ -935,23 +969,23 @@
     @offset.setter
     def offset(self, offset: int) -> None: ...
     @property
     def data_type(self) -> ScalarType: ...
     @data_type.setter
     def data_type(self, data_type: ScalarType) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Sharing:
     def __new__(
         cls,
         name: str,
         offsets: Sequence[Offset],
@@ -976,110 +1010,112 @@
     @size.setter
     def size(self, vector: Vector) -> None: ...
     @property
     def sharing(self) -> Optional[Sharing]: ...
     @sharing.setter
     def sharing(self, sharing: Optional[Sharing]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Vector:
     def __new__(cls, data_type: ScalarType, length: int) -> Self: ...
     @property
     def data_type(self) -> ScalarType: ...
     @data_type.setter
     def data_type(self, data_type: ScalarType) -> None: ...
     @property
     def length(self) -> int: ...
     @length.setter
     def length(self, data_type: int) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class ScalarType(Enum):
     Bit = "BIT"
     Integer = "INTEGER"
     Octet = "OCTET"
     Real = "REAL"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 @final
 class AttributeValue:
-    """
-    A frame attribute value.
+    """A frame attribute value.
 
     # Variants:
     - ``string``: A string attribute containing a ``str``.
     - ``expression``: An expression attribute containing an ``Expression``.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the ``AttributeValue`` is that variant, ``False`` otherwise.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``AttributeValue`` of the given variant from an instance of the inner type.
     """
 
     def inner(self) -> Union[str, Expression]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_string(self) -> bool: ...
     def is_expression(self) -> bool: ...
     @staticmethod
-    def from_string(inner: str) -> "AttributeValue": ...
+    def from_string(inner: str) -> AttributeValue: ...
     @staticmethod
-    def from_expression(inner: Expression) -> "AttributeValue": ...
+    def from_expression(inner: Expression) -> AttributeValue: ...
     def as_string(self) -> Optional[str]: ...
     def to_string(self) -> str: ...
     def as_expression(self) -> Optional[Expression]: ...
     def to_expression(self) -> Expression: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class FrameDefinition:
     def __new__(
         cls,
         identifier: FrameIdentifier,
         attributes: Dict[str, AttributeValue],
@@ -1089,49 +1125,54 @@
     @identifier.setter
     def identifier(self, identifier: FrameIdentifier) -> None: ...
     @property
     def attributes(self) -> Dict[str, AttributeValue]: ...
     @attributes.setter
     def attributes(self, identifier: Dict[str, AttributeValue]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class FrameIdentifier:
     def __new__(cls, name: str, qubits: Sequence[Qubit]) -> Self: ...
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def qubits(self) -> List[Qubit]: ...
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Capture:
     def __new__(
         cls,
         blocking: bool,
         frame: FrameIdentifier,
@@ -1151,26 +1192,31 @@
     @memory_reference.setter
     def memory_reference(self, memory_reference: MemoryReference) -> None: ...
     @property
     def waveform(self) -> WaveformInvocation: ...
     @waveform.setter
     def waveform(self, waveform: WaveformInvocation) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Pulse:
     def __new__(
         cls,
         blocking: bool,
@@ -1186,26 +1232,31 @@
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def waveform(self) -> WaveformInvocation: ...
     @waveform.setter
     def waveform(self, waveform: WaveformInvocation) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class RawCapture:
     def __new__(
         cls,
         blocking: bool,
@@ -1226,205 +1277,240 @@
     @duration.setter
     def duration(self, duration: Expression) -> None: ...
     @property
     def memory_reference(self) -> MemoryReference: ...
     @memory_reference.setter
     def memory_reference(self, memory_reference: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SetFrequency:
     def __new__(cls, frame: FrameIdentifier, frequency: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def frequency(self) -> Expression: ...
     @frequency.setter
     def frequency(self, frequency: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SetPhase:
     def __new__(cls, frame: FrameIdentifier, phase: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def phase(self) -> Expression: ...
     @phase.setter
     def phase(self, phase: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SetScale:
     def __new__(cls, frame: FrameIdentifier, phase: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def scale(self) -> Expression: ...
     @scale.setter
     def scale(self, scale: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class ShiftFrequency:
     def __new__(cls, frame: FrameIdentifier, frequency: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def frequency(self) -> Expression: ...
     @frequency.setter
     def frequency(self, frequency: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class ShiftPhase:
     def __new__(cls, frame: FrameIdentifier, phase: Expression) -> Self: ...
     @property
     def frame(self) -> FrameIdentifier: ...
     @frame.setter
     def frame(self, frame: FrameIdentifier) -> None: ...
     @property
     def phase(self) -> Expression: ...
     @phase.setter
     def phase(self, phase: Expression) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class SwapPhases:
     def __new__(cls, frame_1: FrameIdentifier, frame_2: FrameIdentifier) -> Self: ...
     @property
     def frame_1(self) -> FrameIdentifier: ...
     @frame_1.setter
     def frame_1(self, frame_1: FrameIdentifier) -> None: ...
     @property
     def frame_2(self) -> FrameIdentifier: ...
     @frame_2.setter
     def frame_2(self, frame_2: FrameIdentifier) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class GateError(ValueError):
-    """An error that may occur when performing operations on a ``Gate``"""
+    """An error that may occur when performing operations on a ``Gate``."""
 
     ...
 
 @final
 class GateModifier(Enum):
     Controlled = "CONTROLLED"
     Dagger = "DAGGER"
     Forked = "FORKED"
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Gate:
     def __new__(
         cls,
         name: str,
         parameters: Sequence[Expression],
@@ -1444,67 +1530,63 @@
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     @property
     def modifiers(self) -> List[GateModifier]: ...
     @modifiers.setter
     def modifiers(self, modifiers: Sequence[GateModifier]) -> None: ...
     def dagger(self) -> Self:
-        """
-        Returns a copy of the gate with the ``DAGGER`` modifier added to it.
-        """
+        """Returns a copy of the gate with the ``DAGGER`` modifier added to it."""
         ...
     def controlled(self, control_qubit: Qubit) -> Self:
-        """
-        Returns a copy of the gate with the ``CONTROLLED`` modifier added to it.
-        """
+        """Returns a copy of the gate with the ``CONTROLLED`` modifier added to it."""
     def forked(self, fork_qubit: Qubit, alt_params: Sequence[Expression]) -> Self:
-        """
-        Returns a copy of the gate with the ``FORKED`` modifier added to it.
+        """Returns a copy of the gate with the ``FORKED`` modifier added to it.
 
         Raises a ``GateError`` if the number of provided alternate parameters don't
         equal the number of existing parameters.
         """
         ...
     def to_unitary_mut(self, n_qubits: int) -> NDArray[np.complex_]:
-        """
-        Lift a Gate to the full `n_qubits`-qubit Hilbert space.
+        """Lift a Gate to the full `n_qubits`-qubit Hilbert space.
 
         Returns a ``GateError` if any of the parameters of this gate are
         non-constant, if any of the qubits are variable, if the name of this
         gate is unknown, or if there are an unexpected number of parameters.
         """
         ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class PauliGate(Enum):
     I = "I"
     X = "X"
     Y = "Y"
     Z = "Z"
     @staticmethod
-    def parse(input: str) -> "PauliGate":
-        """
-        Parses a ``PauliGate`` from a string. Raises a ``ParseEnumError`` if the
-        string isn't a valid Pauli word.
-        """
+    def parse(input: str) -> PauliGate:
+        """Parses a ``PauliGate`` from a string. Raises a ``ParseEnumError`` if the string isn't a valid Pauli word."""
         ...
 
 class PauliTerm:
     def __new__(
         cls,
         arguments: Sequence[Tuple[PauliGate, str]],
         expression: Expression,
@@ -1527,58 +1609,55 @@
     @property
     def terms(self) -> List[PauliTerm]: ...
     @terms.setter
     def terms(self, terms: Sequence[PauliTerm]) -> None: ...
 
 @final
 class GateSpecification:
-    """
-    A specification for a gate definition.
+    """A specification for a gate definition.
 
     # Variants:
-    - ``matrix``: A gate specificied by a matrix of ``Expression``s representing a unitary operation.
+    - ``matrix``: A gate specified by a matrix of ``Expression``s representing a unitary operation.
     - ``permutation``: A gate specified by a vector of integers that defines a permutation.
 
     Methods (for each variant):
     - is_*: Returns ``True`` if the inner type is of that variant.
     - as_*: Returns the inner data if it is the given variant, ``None`` otherwise.
     - to_*: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - from_*: Creates a new ``GateSpecification`` using an instance of the inner type for the variant.
     """
 
     def inner(self) -> Union[List[List[Expression]], List[int], PauliSum]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_matrix(self) -> bool: ...
     def is_permutation(self) -> bool: ...
     def is_pauli_sum(self) -> bool: ...
     def as_matrix(self) -> Optional[List[List[Expression]]]: ...
     def to_matrix(self) -> List[List[Expression]]: ...
     def as_permutation(self) -> Optional[List[int]]: ...
     def to_permutation(self) -> List[int]: ...
     def as_pauli_sum(self) -> Optional[PauliSum]: ...
     def to_pauli_sum(self) -> PauliSum: ...
     @staticmethod
-    def from_matrix(inner: Sequence[Sequence[Expression]]) -> "GateSpecification": ...
+    def from_matrix(inner: Sequence[Sequence[Expression]]) -> GateSpecification: ...
     @staticmethod
-    def from_permutation(inner: Sequence[int]) -> "GateSpecification": ...
+    def from_permutation(inner: Sequence[int]) -> GateSpecification: ...
     @staticmethod
-    def from_pauli_sum(inner: PauliSum) -> "GateSpecification": ...
+    def from_pauli_sum(inner: PauliSum) -> GateSpecification: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class GateDefinition:
     def __new__(
         cls,
         name: str,
         parameters: Sequence[str],
@@ -1593,105 +1672,112 @@
     @parameters.setter
     def parameters(self, parameters: Sequence[str]) -> None: ...
     @property
     def specification(self) -> GateSpecification: ...
     @specification.setter
     def specification(self, specification: GateSpecification) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class Qubit:
-    """
-    A Qubit
+    """A Qubit.
 
     # Variants:
     - ``fixed``: A qubit represented as a fixed integer index.
     - ``variable``: A qubit represented by a name.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the inner type is of that variant.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``Qubit`` using an instance of the inner type for the variant.
     """
 
     def inner(self) -> Union[int, str]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_fixed(self) -> bool: ...
     def is_variable(self) -> bool: ...
     def is_placeholder(self) -> bool: ...
     def as_fixed(self) -> Optional[int]: ...
     def to_fixed(self) -> int: ...
     def as_variable(self) -> Optional[str]: ...
     def to_variable(self) -> str: ...
     def as_placeholder(self) -> Optional[QubitPlaceholder]: ...
     def to_placeholder(self) -> QubitPlaceholder: ...
     @staticmethod
-    def from_fixed(inner: int) -> "Qubit": ...
+    def from_fixed(inner: int) -> Qubit: ...
     @staticmethod
-    def from_variable(inner: str) -> "Qubit": ...
+    def from_variable(inner: str) -> Qubit: ...
     @staticmethod
-    def from_placeholder(inner: QubitPlaceholder) -> "Qubit": ...
+    def from_placeholder(inner: QubitPlaceholder) -> Qubit: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class QubitPlaceholder:
-    """
-    A qubit that can be used as a placeholder. Must be resolved before converting
-    a program to valid Quil. See ``quil.program.Program#resolve_placeholders``.
+    """A qubit that can be used as a placeholder.
+
+    Placeholders must be resolved before converting a program to valid Quil. See ``quil.program.Program#resolve_placeholders``.
     """
 
     def __new__(cls) -> Self: ...
     def __lt__(self, other: QubitPlaceholder) -> bool: ...
 
 class Reset:
     def __new__(cls, qubit: Optional[Qubit]) -> Self: ...
     @property
     def qubit(self) -> Optional[Qubit]: ...
     @qubit.setter
     def qubit(self, qubit: Optional[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Delay:
     def __new__(cls, duration: Expression, frame_names: Sequence[str], qubits: Sequence[Qubit]) -> Self: ...
     @property
     def duration(self) -> Expression: ...
@@ -1702,112 +1788,125 @@
     @frame_names.setter
     def frame_names(self, frame_names: Sequence[str]) -> None: ...
     @property
     def qubits(self) -> List[Qubit]: ...
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Fence:
     def __new__(cls, qubits: Sequence[Qubit]) -> Self: ...
     @property
     def qubits(self) -> List[Qubit]: ...
     @qubits.setter
     def qubits(self, qubits: Sequence[Qubit]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class PragmaArgument:
-    """
+    """A PRAGMA argument.
 
-    # Variants:
+    Variants:
     - ``identifier``: A Pragma argument defined by a Quil identifier
     - ``integer``: A Pragma argument defined by an integer
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the inner type is of that variant.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``PragmaArgument`` using an instance of the inner type for the variant.
     """
 
     def inner(self) -> Union[str, int]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     def is_identifier(self) -> bool: ...
     def is_integer(self) -> bool: ...
     def as_identifier(self) -> Optional[str]: ...
     def as_integer(self) -> Optional[int]: ...
     def to_identifier(self) -> str: ...
     def to_integer(self) -> int: ...
     @staticmethod
-    def from_identifier(inner: str) -> "PragmaArgument": ...
+    def from_identifier(inner: str) -> PragmaArgument: ...
     @staticmethod
-    def from_integer(inner: int) -> "PragmaArgument": ...
+    def from_integer(inner: int) -> PragmaArgument: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Include:
     def __new__(cls, filename: str) -> Self: ...
     @property
     def filename(self) -> str: ...
     @filename.setter
     def filename(self, filename: str) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Pragma:
     def __new__(cls, name: str, arguments: Sequence[PragmaArgument], data: Optional[str]) -> Self: ...
     @property
     def name(self) -> str: ...
@@ -1818,85 +1917,95 @@
     @arguments.setter
     def arguments(self, arguments: Sequence[PragmaArgument]) -> None: ...
     @property
     def data(self) -> Optional[str]: ...
     @data.setter
     def data(self, data: Optional[str]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Measurement:
     def __new__(cls, qubit: Qubit, target: Optional[MemoryReference]) -> Self: ...
     @property
     def qubit(self) -> Qubit: ...
     @qubit.setter
     def qubit(self, qubit: Qubit) -> None: ...
     @property
     def target(self) -> Optional[MemoryReference]: ...
     @target.setter
     def target(self, target: Optional[MemoryReference]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class ParseMemoryReferenceError(ValueError):
-    """Errors that may occur while parsing a ``MemoryReference``"""
+    """Errors that may occur while parsing a ``MemoryReference``."""
 
 class MemoryReference:
     def __new__(cls, name: str, index: int) -> Self: ...
     @staticmethod
-    def parse(input: str) -> "MemoryReference":
-        """
-        Parses a ``MemoryReference`` from a string. Raises a ``ParseMemoryReference`` error if the
-        string isn't a valid Quil memory reference.
+    def parse(input: str) -> MemoryReference:
+        """Parses a ``MemoryReference`` from a string.
+
+        Raises a ``ParseMemoryReference`` error if the string isn't a valid Quil memory reference.
         """
         ...
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def index(self) -> int: ...
     @index.setter
     def index(self, index: int) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Load:
     def __new__(cls, destination: MemoryReference, source: str, offset: MemoryReference) -> Self: ...
     @property
     def destination(self) -> MemoryReference: ...
     @destination.setter
@@ -1906,26 +2015,31 @@
     @source.setter
     def source(self, source: str) -> None: ...
     @property
     def offset(self) -> MemoryReference: ...
     @offset.setter
     def offset(self, offset: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Store:
     def __new__(cls, destination: str, offset: MemoryReference, source: ArithmeticOperand) -> Self: ...
     @property
     def destination(self) -> str: ...
@@ -1936,26 +2050,31 @@
     @offset.setter
     def offset(self, offset: MemoryReference) -> None: ...
     @property
     def source(self) -> ArithmeticOperand: ...
     @source.setter
     def source(self, source: ArithmeticOperand) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class Waveform:
     def __new__(cls, matrix: Sequence[Expression], parameters: Sequence[str]) -> Self: ...
     @property
     def matrix(self) -> List[Expression]: ...
@@ -1973,117 +2092,124 @@
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def definition(self) -> Waveform: ...
     @definition.setter
     def definition(self, definition: Waveform) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class WaveformInvocation:
     def __new__(cls, name: str, parameters: Dict[str, Expression]) -> Self: ...
     @property
     def name(self) -> str: ...
     @name.setter
     def name(self, name: str) -> None: ...
     @property
     def parameters(self) -> Dict[str, Expression]: ...
     @parameters.setter
     def parameters(self, parameters: Dict[str, Expression]) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class Label:
     def __new__(cls, target: Target) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 @final
 class Target:
-    """
-    Represents a Quil target.
+    """Represents a Quil target.
 
     # Variants:
     - ``fixed``: A fixed target defined by a Quil identifier
     - ``placeholder``: A placeholder target that can be assigned a new name at a later time.
 
     Methods (for each variant):
     - ``is_*``: Returns ``True`` if the inner type is of that variant.
     - ``as_*``: Returns the inner data if it is the given variant, ``None`` otherwise.
     - ``to_*``: Returns the inner data if it is the given variant, raises ``ValueError`` otherwise.
     - ``from_*``: Creates a new ``PragmaArgument`` using an instance of the inner type for the variant.
     """
 
-    def __new__(cls, inner: Union[str, TargetPlaceholder]) -> "Target": ...
+    def __new__(cls, inner: Union[str, TargetPlaceholder]) -> Target: ...
     @staticmethod
-    def from_fixed(inner: str) -> "Target": ...
+    def from_fixed(inner: str) -> Target: ...
     @staticmethod
-    def from_placeholder(inner: TargetPlaceholder) -> "Target": ...
+    def from_placeholder(inner: TargetPlaceholder) -> Target: ...
     def is_fixed(self) -> bool: ...
     def is_placeholder(self) -> bool: ...
     def as_fixed(self) -> Optional[str]: ...
     def as_placeholder(self) -> Optional[TargetPlaceholder]: ...
     def to_fixed(self) -> str: ...
     def to_placeholder(self) -> TargetPlaceholder: ...
     def inner(self) -> Union[str, TargetPlaceholder]: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
 
 class TargetPlaceholder:
-    """
-    A placeholder target that must be assigned a fixed name before creating a program
-    with valid quil.
+    """A placeholder target that must be assigned a fixed name before creating a program with valid quil.
 
     See ``quil.program.Program#resolve_placeholders`` for more information.
     """
 
     def __new__(cls, base_target: str) -> Self: ...
     @property
     def base_label(self) -> str: ...
@@ -2091,73 +2217,88 @@
 class Jump:
     def __new__(cls, target: Target) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class JumpWhen:
     def __new__(cls, target: Target, condition: MemoryReference) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     @property
     def condition(self) -> MemoryReference: ...
     @condition.setter
     def condition(self, condition: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
 
 class JumpUnless:
     def __new__(cls, target: Target, condition: MemoryReference) -> Self: ...
     @property
     def target(self) -> Target: ...
     @target.setter
     def target(self, target: Target) -> None: ...
     @property
     def condition(self) -> MemoryReference: ...
     @condition.setter
     def condition(self, condition: MemoryReference) -> None: ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
+        """Attempt to convert the instruction to a valid Quil string.
+
+        Raises an exception if the instruction can't be converted to valid Quil.
         """
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug format.
         """
     def __deepcopy__(self, _: Dict) -> Self:
-        """Creates and returns a deep copy of the class. If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with new placeholders so resolving them in the copy will not resolve them in the original.  Should be used by passing an instance of the class to ``copy.deepcopy``"""
+        """Creates and returns a deep copy of the class.
+
+        If the instruction contains any ``QubitPlaceholder`` or ``TargetPlaceholder``, then they will be replaced with
+        new placeholders so resolving them in the copy will not resolve them in the original.
+        Should be used by passing an instance of the class to ``copy.deepcopy``
+        """
     def __copy__(self) -> Self:
         """Returns a shallow copy of the class."""
```

### Comparing `quil-0.9.0rc0/quil/expression/__init__.pyi` & `quil-0.9.1rc0/quil/expression/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""
-The ``expression`` module contains classes for representing Quil expressions.
-"""
+"""The ``expression`` module contains classes for representing Quil expressions."""
+
 from enum import Enum
-from typing import Dict, final, Sequence, Optional, Union
+from typing import Dict, Optional, Sequence, Union, final
 
 from quil.instructions import MemoryReference
 
 class EvaluationError(ValueError):
-    """Error that may occur while evaluation an ``Expression``"""
+    """Error that may occur while evaluation an ``Expression``."""
 
 class ParseExpressionError(ValueError):
-    """Error that may occur while parsing an ``Expression``"""
+    """Error that may occur while parsing an ``Expression``."""
 
 @final
 class Expression:
-    """
-    A Quil expression.
+    """A Quil expression.
 
     # Variants:
     - ``address``: An address defined by a `quil.instructions.MemoryReference`.
     - ``function_call``: A `FunctionCallExpression`.
     - ``infix``: An `InfixExpression`.
     - ``number``: A number defined as a `complex`.
     - ``pi``: The constant ``pi``. No inner data.
@@ -41,24 +39,29 @@
 
     If the variant doesn't have inner data (e.g. ``pi``)
     - ``new_*``: Creates a new ``Expression`` for the variant
     """
 
     def inner(
         self,
-    ) -> Union[MemoryReference, FunctionCallExpression, InfixExpression, int, PrefixExpression, str,]:
-        """
-        Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist.
-        """
+    ) -> Union[
+        MemoryReference,
+        FunctionCallExpression,
+        InfixExpression,
+        int,
+        PrefixExpression,
+        str,
+    ]:
+        """Returns the inner value of the variant. Raises a ``RuntimeError`` if inner data doesn't exist."""
         ...
     @staticmethod
     def parse(input: str) -> Expression:
-        """
-        Parses an ``Expression`` from a string. Raises a ``ParseExpressionError`` if the string
-        isn't a valid Quil expression.
+        """Parses an ``Expression`` from a string.
+
+        Raises a ``ParseExpressionError`` if the string isn't a valid Quil expression.
         """
     def is_address(self) -> bool: ...
     def is_function_call(self) -> bool: ...
     def is_infix(self) -> bool: ...
     def is_number(self) -> bool: ...
     def is_pi(self) -> bool: ...
     def is_prefix(self) -> bool: ...
@@ -86,79 +89,62 @@
     def as_number(self) -> Optional[complex]: ...
     def to_number(self) -> complex: ...
     def as_prefix(self) -> Optional[PrefixExpression]: ...
     def to_prefix(self) -> PrefixExpression: ...
     def as_variable(self) -> Optional[str]: ...
     def to_variable(self) -> str: ...
     def simplify(self):
-        """
-        Simplify the expression as much as possible, in-place.
-        """
+        """Simplify the expression as much as possible, in-place."""
         ...
     def into_simplified(self) -> "Expression":
-        """
-        Return a simplified copy of the expression.
-        """
+        """Return a simplified copy of the expression."""
     def evaluate(
         self,
         variables: Dict[str, complex],
         memory_references: Dict[str, Sequence[float]],
     ) -> complex:
-        """
-        Evaluate an expression, expecting that it may be fully reduced to a single complex number.
+        """Evaluate an expression, expecting that it may be fully reduced to a single complex number.
+
         If it cannot be reduced to a complex number, raises an ``EvaluationError``.
         """
         ...
     def substitute_variables(self, variable_values: Dict[str, "Expression"]) -> "Expression":
-        """
-        Returns a copy of the expression where every matching variable in `variable_values` is
-        replaced by the corresponding expression.
-        """
+        """Returns a copy of the expression where every matching variable in `variable_values` is replaced by the corresponding expression."""
         ...
     def to_real(self) -> float:
-        """
-        If this is a number with imaginary part "equal to" zero (of <em>small</em> absolute value), return
-        that number. Otherwise, raises an ``EvaluationError``
-        """
+        """If this is a number with imaginary part "equal to" zero (of <em>small</em> absolute value), return that number. Otherwise, raises an ``EvaluationError``."""
     def __add__(self, other: "Expression") -> "Expression": ...
     def __sub__(self, other: "Expression") -> "Expression": ...
     def __mul__(self, other: "Expression") -> "Expression": ...
     def __truediv__(self, other: "Expression") -> "Expression": ...
     def to_quil(self) -> str:
-        """
-        Attempt to convert the instruction to a valid Quil string. Raises
-        an exception if the instruction can't be converted to valid Quil.
-        """
+        """Attempt to convert the instruction to a valid Quil string. Raises an exception if the instruction can't be converted to valid Quil."""
         ...
     def to_quil_or_debug(self) -> str:
-        """
-        Convert the instruction to a Quil string. If any part of the instruction can't
-        be converted to valid Quil, it will be printed in a human-readable debug format
-        that isn't valid Quil.
+        """Convert the instruction to a Quil string.
+
+        If any part of the instruction can't be converted to valid Quil, it will be printed in a human-readable debug
+        format that isn't valid Quil.
         """
 
 class FunctionCallExpression:
-    """
-    A Quil function call.
-    """
+    """A Quil function call."""
     @staticmethod
     def __new__(cls, function: ExpressionFunction, expression: Expression) -> "FunctionCallExpression": ...
     @property
     def function(self) -> ExpressionFunction: ...
     @function.setter
     def function(self, function: ExpressionFunction): ...
     @property
     def expression(self) -> Expression: ...
     @expression.setter
     def expression(self, expression: Expression): ...
 
 class InfixExpression:
-    """
-    A Quil infix expression.
-    """
+    """A Quil infix expression."""
     @staticmethod
     def __new__(cls, left: Expression, operator: InfixOperator, right: Expression): ...
     @property
     def left(self) -> Expression: ...
     @left.setter
     def left(self, expression: Expression): ...
     @property
@@ -167,50 +153,45 @@
     def operator(self, operator: InfixOperator): ...
     @property
     def right(self) -> Expression: ...
     @right.setter
     def right(self, expression: Expression): ...
 
 class PrefixExpression:
-    """
-    A Quil prefix expression.
-    """
+    """A Quil prefix expression."""
     @staticmethod
     def __new__(cls, operator: PrefixOperator, expression: Expression): ...
     @property
     def operator(self) -> PrefixOperator: ...
     @operator.setter
     def operator(self, operator: PrefixOperator): ...
     @property
     def expression(self) -> Expression: ...
     @expression.setter
     def expression(self, expression: Expression): ...
 
 @final
 class ExpressionFunction(Enum):
-    """
-    An enum representing a Quil function that can be applied to an expression.
-    """
+    """An enum representing a Quil function that can be applied to an expression."""
+
     Cis = "CIS"
     Cosine = "COSINE"
     Exponent = "EXPONENT"
     Sine = "SINE"
     SquareRoot = "SQUAREROOT"
 
 @final
 class PrefixOperator(Enum):
-    """
-    An enum that represents the operators supported on a prefix expression.
-    """
+    """An enum that represents the operators supported on a prefix expression."""
+
     Plus = "PLUS"
     Minus = "MINUS"
 
 @final
 class InfixOperator(Enum):
-    """
-    An enum that represents the operators supported on an infix expression.
-    """
+    """An enum that represents the operators supported on an infix expression."""
+
     Caret = "CARET"
     Plus = "PLUS"
     Minus = "MINUS"
     Slash = "SLASH"
     Star = "STAR"
```

### Comparing `quil-0.9.0rc0/README-py.md` & `quil-0.9.1rc0/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.9.0rc0/PKG-INFO` & `quil-0.9.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quil
-Version: 0.9.0rc0
+Version: 0.9.1rc0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Summary: A Python package for building and parsing Quil programs.
```

