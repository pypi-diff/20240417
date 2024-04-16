# Comparing `tmp/quil-0.8.0.tar.gz` & `tmp/quil-0.9.0rc0.tar.gz`

## Comparing `quil-0.8.0.tar` & `quil-0.9.0rc0.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0     1001      127     1414 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/Cargo.toml
--rw-r--r--   0     1001      127    43787 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/CHANGELOG.md
--rw-r--r--   0     1001      127      954 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/README.md
--rw-r--r--   0     1001      127     1692 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/corpus.rs
--rw-r--r--   0     1001      127      941 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/get_frames_for_instruction.rs
--rw-r--r--   0     1001      127      985 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/parser.rs
--rw-r--r--   0     1001      127   803952 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/sample-calibrations.quil
--rw-r--r--   0     1001      127     1478 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/scheduled_program_from_program.rs
--rw-r--r--   0     1001      127      969 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/simplification.rs
--rw-r--r--   0     1001      127    12979 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/test_expressions.txt
--rw-r--r--   0     1001      127     6316 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/examples/generate_test_expressions.rs
--rw-r--r--   0     1001      127    38082 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/expression/mod.rs
--rw-r--r--   0     1001      127    34338 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/expression/simplification/by_hand.rs
--rw-r--r--   0     1001      127    12745 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/expression/simplification/mod.rs
--rw-r--r--   0     1001      127     1002 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/hash.rs
--rw-r--r--   0     1001      127     5302 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     6478 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/circuit.rs
--rw-r--r--   0     1001      127     9937 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/classical.rs
--rw-r--r--   0     1001      127     5260 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     6939 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9857 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/frame.rs
--rw-r--r--   0     1001      127    43954 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/gate.rs
--rw-r--r--   0     1001      127      771 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/measurement.rs
--rw-r--r--   0     1001      127    39423 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1798 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/pragma.rs
--rw-r--r--   0     1001      127     3425 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      654 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/reset.rs
--rw-r--r--   0     1001      127      133 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
--rw-r--r--   0     1001      127      133 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
--rw-r--r--   0     1001      127      124 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
--rw-r--r--   0     1001      127      167 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
--rw-r--r--   0     1001      127      160 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
--rw-r--r--   0     1001      127      109 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
--rw-r--r--   0     1001      127      141 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
--rw-r--r--   0     1001      127      125 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
--rw-r--r--   0     1001      127      191 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
--rw-r--r--   0     1001      127      178 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
--rw-r--r--   0     1001      127      139 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
--rw-r--r--   0     1001      127      143 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
--rw-r--r--   0     1001      127     1528 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/timing.rs
--rw-r--r--   0     1001      127     3619 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1910 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/lib.rs
--rw-r--r--   0     1001      127     1013 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/macros.rs
--rw-r--r--   0     1001      127    36217 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/command.rs
--rw-r--r--   0     1001      127    23037 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/common.rs
--rw-r--r--   0     1001      127     5970 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/error.rs
--rw-r--r--   0     1001      127     2519 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/input.rs
--rw-r--r--   0     1001      127     3242 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/internal.rs
--rw-r--r--   0     1001      127     1004 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/kind.rs
--rw-r--r--   0     1001      127     2685 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/mod.rs
--rw-r--r--   0     1001      127    17487 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/expression.rs
--rw-r--r--   0     1001      127     2212 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/gate.rs
--rw-r--r--   0     1001      127    40956 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/instruction.rs
--rw-r--r--   0     1001      127     1380 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/error.rs
--rw-r--r--   0     1001      127    17439 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/mod.rs
--rw-r--r--   0     1001      127     4222 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/quoted_strings.rs
--rw-r--r--   0     1001      127     3357 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/wrapped_parsers.rs
--rw-r--r--   0     1001      127     4162 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/macros.rs
--rw-r--r--   0     1001      127     2446 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/mod.rs
--rw-r--r--   0     1001      127     5841 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/token.rs
--rw-r--r--   0     1001      127    25985 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/control_flow_graph.rs
--rw-r--r--   0     1001      127      974 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/mod.rs
--rw-r--r--   0     1001      127     9591 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/qubit_graph.rs
--rw-r--r--   0     1001      127      889 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
--rw-r--r--   0     1001      127     1329 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/test_programs.rs
--rw-r--r--   0     1001      127    23626 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/calibration.rs
--rw-r--r--   0     1001      127     8286 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/calibration_set.rs
--rw-r--r--   0     1001      127     2283 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/leftover.rs
--rw-r--r--   0     1001      127     3068 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/mod.rs
--rw-r--r--   0     1001      127     2252 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/result.rs
--rw-r--r--   0     1001      127     2725 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/syntax.rs
--rw-r--r--   0     1001      127     8742 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/frame.rs
--rw-r--r--   0     1001      127    17109 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/memory.rs
--rw-r--r--   0     1001      127    48872 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/mod.rs
--rw-r--r--   0     1001      127    26031 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/graph.rs
--rw-r--r--   0     1001      127    20046 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/graphviz_dot.rs
--rw-r--r--   0     1001      127      456 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/mod.rs
--rw-r--r--   0     1001      127    16670 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/schedule.rs
--rw-r--r--   0     1001      127     2678 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
--rw-r--r--   0     1001      127     1560 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
--rw-r--r--   0     1001      127     1166 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
--rw-r--r--   0     1001      127     1732 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
--rw-r--r--   0     1001      127     1112 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
--rw-r--r--   0     1001      127     1195 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
--rw-r--r--   0     1001      127     1780 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
--rw-r--r--   0     1001      127     1653 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
--rw-r--r--   0     1001      127     1003 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
--rw-r--r--   0     1001      127     1032 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
--rw-r--r--   0     1001      127      552 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
--rw-r--r--   0     1001      127     1540 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
--rw-r--r--   0     1001      127     1073 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
--rw-r--r--   0     1001      127     1338 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
--rw-r--r--   0     1001      127     1866 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
--rw-r--r--   0     1001      127      854 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
--rw-r--r--   0     1001      127      867 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
--rw-r--r--   0     1001      127      887 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
--rw-r--r--   0     1001      127     1892 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
--rw-r--r--   0     1001      127      839 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
--rw-r--r--   0     1001      127      768 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
--rw-r--r--   0     1001      127      591 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
--rw-r--r--   0     1001      127      793 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
--rw-r--r--   0     1001      127      852 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
--rw-r--r--   0     1001      127      585 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
--rw-r--r--   0     1001      127      227 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
--rw-r--r--   0     1001      127      136 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
--rw-r--r--   0     1001      127      215 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
--rw-r--r--   0     1001      127      476 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
--rw-r--r--   0     1001      127      210 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
--rw-r--r--   0     1001      127      141 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
--rw-r--r--   0     1001      127      159 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
--rw-r--r--   0     1001      127      309 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
--rw-r--r--   0     1001      127      261 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
--rw-r--r--   0     1001      127      155 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
--rw-r--r--   0     1001      127      254 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
--rw-r--r--   0     1001      127      174 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
--rw-r--r--   0     1001      127      167 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
--rw-r--r--   0     1001      127     3755 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
--rw-r--r--   0     1001      127      425 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
--rw-r--r--   0     1001      127    35007 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/type_check.rs
--rw-r--r--   0     1001      127     2422 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/quil.rs
--rw-r--r--   0     1001      127     2749 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/reserved.rs
--rw-r--r--   0     1001      127     2109 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/validation/identifier.rs
--rw-r--r--   0     1001      127       20 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/validation/mod.rs
--rw-r--r--   0     1001      127      724 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/calibration_test.rs
--rw-r--r--   0     1001      127      742 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_cz.quil
--rw-r--r--   0     1001      127     1888 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_cz_phase.quil
--rw-r--r--   0     1001      127     3266 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_measure.quil
--rw-r--r--   0     1001      127     1588 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_rx.quil
--rw-r--r--   0     1001      127     1786 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_xy.quil
--rw-r--r--   0     1001      127      747 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
--rw-r--r--   0     1001      127     1797 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
--rw-r--r--   0     1001      127     3187 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
--rw-r--r--   0     1001      127     1519 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
--rw-r--r--   0     1001      127     1719 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 quil-0.8.0/quil-py/Cargo.toml
--rw-r--r--   0     1001      127      203 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/.flake8
--rw-r--r--   0     1001      127       10 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/.stubtest-allowlist
--rw-r--r--   0     1001      127    20226 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/CHANGELOG.md
--rw-r--r--   0     1001      127      858 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/Makefile.toml
--rw-r--r--   0     1001      127      777 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/README-py.md
--rw-r--r--   0     1001      127      337 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/README.md
--rw-r--r--   0     1001      127       71 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/build.rs
--rw-r--r--   0     1001      127      404 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/make_docs.py
--rw-r--r--   0     1001      127      135 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/index.html
--rw-r--r--   0     1001      127    34673 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/quil/quil.html
--rw-r--r--   0     1001      127    34581 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/quil.html
--rw-r--r--   0     1001      127    20706 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/search.js
--rw-r--r--   0     1001      127    36038 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/poetry.lock
--rw-r--r--   0     1001      127      283 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/__init__.pyi
--rw-r--r--   0     1001      127       30 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7690 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127      124 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91321 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127      129 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/program/__init__.py
--rw-r--r--   0     1001      127    18326 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/program/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/py.typed
--rw-r--r--   0     1001      127      161 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/__init__.py
--rw-r--r--   0     1001      127       39 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127       41 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/identifier.py
--rw-r--r--   0     1001      127      439 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127    34593 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil.html
--rw-r--r--   0     1001      127     6656 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/expression.rs
--rw-r--r--   0     1001      127     2838 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     1251 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/circuit.rs
--rw-r--r--   0     1001      127    11440 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/classical.rs
--rw-r--r--   0     1001      127     4295 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     5561 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9528 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/frame.rs
--rw-r--r--   0     1001      127     8394 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/gate.rs
--rw-r--r--   0     1001      127     1056 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/measurement.rs
--rw-r--r--   0     1001      127     8741 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1852 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/pragma.rs
--rw-r--r--   0     1001      127      978 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      738 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/reset.rs
--rw-r--r--   0     1001      127     1591 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/timing.rs
--rw-r--r--   0     1001      127     2434 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1967 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/lib.rs
--rw-r--r--   0     1001      127     2701 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/analysis.rs
--rw-r--r--   0     1001      127     4156 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/calibration.rs
--rw-r--r--   0     1001      127     2774 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/frame.rs
--rw-r--r--   0     1001      127      897 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/memory.rs
--rw-r--r--   0     1001      127    12662 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/mod.rs
--rw-r--r--   0     1001      127     1696 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/scheduling.rs
--rw-r--r--   0     1001      127     1136 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/validation/identifier.rs
--rw-r--r--   0     1001      127      151 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/validation/mod.rs
--rw-r--r--   0     1001      127     1665 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/instructions/test_copy.py
--rw-r--r--   0     1001      127      351 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/instructions/test_gate.py
--rw-r--r--   0     1001      127      137 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/program/__snapshots__/test_program.ambr
--rw-r--r--   0     1001      127     4566 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/program/test_program.py
--rw-r--r--   0     1001      127     1023 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/test_eq.py
--rw-r--r--   0     1001      127    50010 2024-04-15 17:47:41.000000 quil-0.8.0/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 quil-0.8.0/Cargo.toml
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 quil-0.8.0/pyproject.toml
--rw-r--r--   0     1001      127      124 2024-04-15 17:47:41.000000 quil-0.8.0/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91321 2024-04-15 17:47:41.000000 quil-0.8.0/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127      129 2024-04-15 17:47:41.000000 quil-0.8.0/quil/program/__init__.py
--rw-r--r--   0     1001      127    18326 2024-04-15 17:47:41.000000 quil-0.8.0/quil/program/__init__.pyi
--rw-r--r--   0     1001      127      439 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127      161 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/__init__.py
--rw-r--r--   0     1001      127       41 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/identifier.py
--rw-r--r--   0     1001      127       39 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127      283 2024-04-15 17:47:41.000000 quil-0.8.0/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil/py.typed
--rw-r--r--   0     1001      127       30 2024-04-15 17:47:41.000000 quil-0.8.0/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7690 2024-04-15 17:47:41.000000 quil-0.8.0/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil/__init__.pyi
--rw-r--r--   0     1001      127      777 2024-04-15 17:47:41.000000 quil-0.8.0/README-py.md
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 quil-0.8.0/PKG-INFO
+-rw-r--r--   0     1001      127     1419 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/Cargo.toml
+-rw-r--r--   0     1001      127    44103 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/CHANGELOG.md
+-rw-r--r--   0     1001      127      954 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/README.md
+-rw-r--r--   0     1001      127     1692 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/corpus.rs
+-rw-r--r--   0     1001      127      941 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/get_frames_for_instruction.rs
+-rw-r--r--   0     1001      127      985 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/parser.rs
+-rw-r--r--   0     1001      127   803952 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/sample-calibrations.quil
+-rw-r--r--   0     1001      127     1478 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/scheduled_program_from_program.rs
+-rw-r--r--   0     1001      127      969 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/simplification.rs
+-rw-r--r--   0     1001      127    12979 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/benches/test_expressions.txt
+-rw-r--r--   0     1001      127     6316 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/examples/generate_test_expressions.rs
+-rw-r--r--   0     1001      127    38082 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/expression/mod.rs
+-rw-r--r--   0     1001      127    34338 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/expression/simplification/by_hand.rs
+-rw-r--r--   0     1001      127    12745 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/expression/simplification/mod.rs
+-rw-r--r--   0     1001      127     1002 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/hash.rs
+-rw-r--r--   0     1001      127     5302 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     6478 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127     9937 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     5260 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     6939 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9842 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/frame.rs
+-rw-r--r--   0     1001      127    43954 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/gate.rs
+-rw-r--r--   0     1001      127      771 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127    39443 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1798 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127     3425 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      654 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/reset.rs
+-rw-r--r--   0     1001      127      133 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
+-rw-r--r--   0     1001      127      133 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
+-rw-r--r--   0     1001      127      124 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
+-rw-r--r--   0     1001      127      167 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
+-rw-r--r--   0     1001      127      160 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
+-rw-r--r--   0     1001      127      109 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
+-rw-r--r--   0     1001      127      141 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
+-rw-r--r--   0     1001      127      125 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
+-rw-r--r--   0     1001      127      191 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
+-rw-r--r--   0     1001      127      178 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
+-rw-r--r--   0     1001      127      139 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
+-rw-r--r--   0     1001      127      143 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
+-rw-r--r--   0     1001      127     1528 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     3666 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1910 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/lib.rs
+-rw-r--r--   0     1001      127     1013 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/macros.rs
+-rw-r--r--   0     1001      127    36217 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/command.rs
+-rw-r--r--   0     1001      127    23080 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/common.rs
+-rw-r--r--   0     1001      127     5970 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/error.rs
+-rw-r--r--   0     1001      127     2519 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/input.rs
+-rw-r--r--   0     1001      127     3242 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/internal.rs
+-rw-r--r--   0     1001      127     1004 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/kind.rs
+-rw-r--r--   0     1001      127     2685 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/error/mod.rs
+-rw-r--r--   0     1001      127    17487 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/expression.rs
+-rw-r--r--   0     1001      127     2212 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/gate.rs
+-rw-r--r--   0     1001      127    40974 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/instruction.rs
+-rw-r--r--   0     1001      127     1380 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/error.rs
+-rw-r--r--   0     1001      127    17439 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/mod.rs
+-rw-r--r--   0     1001      127     4222 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/quoted_strings.rs
+-rw-r--r--   0     1001      127     3357 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs
+-rw-r--r--   0     1001      127     4162 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/macros.rs
+-rw-r--r--   0     1001      127     2446 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/mod.rs
+-rw-r--r--   0     1001      127     5841 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/parser/token.rs
+-rw-r--r--   0     1001      127    25985 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/control_flow_graph.rs
+-rw-r--r--   0     1001      127      974 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/mod.rs
+-rw-r--r--   0     1001      127     9591 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/qubit_graph.rs
+-rw-r--r--   0     1001      127      889 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
+-rw-r--r--   0     1001      127     1329 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/analysis/test_programs.rs
+-rw-r--r--   0     1001      127    23626 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/calibration.rs
+-rw-r--r--   0     1001      127     7227 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/calibration_set.rs
+-rw-r--r--   0     1001      127     2283 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/leftover.rs
+-rw-r--r--   0     1001      127     3068 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/mod.rs
+-rw-r--r--   0     1001      127     2252 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/result.rs
+-rw-r--r--   0     1001      127     2725 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/error/syntax.rs
+-rw-r--r--   0     1001      127     8742 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/frame.rs
+-rw-r--r--   0     1001      127    17109 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/memory.rs
+-rw-r--r--   0     1001      127    51116 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/mod.rs
+-rw-r--r--   0     1001      127    26031 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/graph.rs
+-rw-r--r--   0     1001      127    20046 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/graphviz_dot.rs
+-rw-r--r--   0     1001      127      456 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/mod.rs
+-rw-r--r--   0     1001      127    16670 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/schedule.rs
+-rw-r--r--   0     1001      127     2678 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
+-rw-r--r--   0     1001      127     1560 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
+-rw-r--r--   0     1001      127     1166 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
+-rw-r--r--   0     1001      127     1732 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
+-rw-r--r--   0     1001      127     1112 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
+-rw-r--r--   0     1001      127     1195 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
+-rw-r--r--   0     1001      127     1780 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
+-rw-r--r--   0     1001      127     1653 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
+-rw-r--r--   0     1001      127     1003 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
+-rw-r--r--   0     1001      127     1032 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
+-rw-r--r--   0     1001      127      552 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
+-rw-r--r--   0     1001      127     1540 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
+-rw-r--r--   0     1001      127     1073 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
+-rw-r--r--   0     1001      127     1338 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
+-rw-r--r--   0     1001      127     1866 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
+-rw-r--r--   0     1001      127      854 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
+-rw-r--r--   0     1001      127      867 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
+-rw-r--r--   0     1001      127      887 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
+-rw-r--r--   0     1001      127     1892 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
+-rw-r--r--   0     1001      127      839 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
+-rw-r--r--   0     1001      127      768 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
+-rw-r--r--   0     1001      127      591 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
+-rw-r--r--   0     1001      127      793 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
+-rw-r--r--   0     1001      127      852 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
+-rw-r--r--   0     1001      127      585 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
+-rw-r--r--   0     1001      127      227 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
+-rw-r--r--   0     1001      127      136 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
+-rw-r--r--   0     1001      127      215 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
+-rw-r--r--   0     1001      127      476 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
+-rw-r--r--   0     1001      127      210 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
+-rw-r--r--   0     1001      127      141 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
+-rw-r--r--   0     1001      127      159 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
+-rw-r--r--   0     1001      127      309 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
+-rw-r--r--   0     1001      127      261 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
+-rw-r--r--   0     1001      127      155 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
+-rw-r--r--   0     1001      127      254 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
+-rw-r--r--   0     1001      127      174 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
+-rw-r--r--   0     1001      127      167 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
+-rw-r--r--   0     1001      127     3755 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
+-rw-r--r--   0     1001      127      425 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
+-rw-r--r--   0     1001      127    35001 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/program/type_check.rs
+-rw-r--r--   0     1001      127     2422 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/quil.rs
+-rw-r--r--   0     1001      127     2749 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/reserved.rs
+-rw-r--r--   0     1001      127     2109 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/validation/identifier.rs
+-rw-r--r--   0     1001      127       20 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/src/validation/mod.rs
+-rw-r--r--   0     1001      127      724 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/calibration_test.rs
+-rw-r--r--   0     1001      127      742 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz.quil
+-rw-r--r--   0     1001      127     1888 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz_phase.quil
+-rw-r--r--   0     1001      127     3266 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_measure.quil
+-rw-r--r--   0     1001      127     1588 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_rx.quil
+-rw-r--r--   0     1001      127     1786 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/programs/calibration_xy.quil
+-rw-r--r--   0     1001      127      747 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
+-rw-r--r--   0     1001      127     1797 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
+-rw-r--r--   0     1001      127     3187 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
+-rw-r--r--   0     1001      127     1519 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
+-rw-r--r--   0     1001      127     1719 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 quil-0.9.0rc0/quil-py/Cargo.toml
+-rw-r--r--   0     1001      127      203 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/.flake8
+-rw-r--r--   0     1001      127       10 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/.stubtest-allowlist
+-rw-r--r--   0     1001      127    20540 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/CHANGELOG.md
+-rw-r--r--   0     1001      127      858 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/Makefile.toml
+-rw-r--r--   0     1001      127      777 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/README-py.md
+-rw-r--r--   0     1001      127      337 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/README.md
+-rw-r--r--   0     1001      127       71 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/build.rs
+-rw-r--r--   0     1001      127      404 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/make_docs.py
+-rw-r--r--   0     1001      127      135 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/index.html
+-rw-r--r--   0     1001      127    34673 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/quil/quil.html
+-rw-r--r--   0     1001      127    34581 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/quil.html
+-rw-r--r--   0     1001      127    20706 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/out/search.js
+-rw-r--r--   0     1001      127    36038 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/poetry.lock
+-rw-r--r--   0     1001      127      283 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/__init__.pyi
+-rw-r--r--   0     1001      127       30 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7690 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127      124 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91321 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127      129 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/program/__init__.py
+-rw-r--r--   0     1001      127    18326 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/py.typed
+-rw-r--r--   0     1001      127      161 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       39 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127       41 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/identifier.py
+-rw-r--r--   0     1001      127      439 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127    34593 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/quil.html
+-rw-r--r--   0     1001      127     6656 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/expression.rs
+-rw-r--r--   0     1001      127     2838 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     1251 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127    11440 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     4295 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     5561 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9507 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/frame.rs
+-rw-r--r--   0     1001      127     8394 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/gate.rs
+-rw-r--r--   0     1001      127     1056 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127     8741 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1852 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127      978 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      738 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/reset.rs
+-rw-r--r--   0     1001      127     1591 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     2443 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1967 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/lib.rs
+-rw-r--r--   0     1001      127     2701 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/analysis.rs
+-rw-r--r--   0     1001      127     4156 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/calibration.rs
+-rw-r--r--   0     1001      127     2774 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/frame.rs
+-rw-r--r--   0     1001      127      897 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/memory.rs
+-rw-r--r--   0     1001      127    12676 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/mod.rs
+-rw-r--r--   0     1001      127     1696 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/program/scheduling.rs
+-rw-r--r--   0     1001      127     1136 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/validation/identifier.rs
+-rw-r--r--   0     1001      127      151 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/src/validation/mod.rs
+-rw-r--r--   0     1001      127     1665 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/instructions/test_copy.py
+-rw-r--r--   0     1001      127      351 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/instructions/test_gate.py
+-rw-r--r--   0     1001      127      137 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/program/__snapshots__/test_program.ambr
+-rw-r--r--   0     1001      127     4566 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/program/test_program.py
+-rw-r--r--   0     1001      127     1023 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil-py/test/test_eq.py
+-rw-r--r--   0     1001      127    50481 2024-04-16 22:48:12.000000 quil-0.9.0rc0/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 quil-0.9.0rc0/Cargo.toml
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 quil-0.9.0rc0/pyproject.toml
+-rw-r--r--   0     1001      127      129 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/program/__init__.py
+-rw-r--r--   0     1001      127    18326 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/py.typed
+-rw-r--r--   0     1001      127      124 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91321 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127       30 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7690 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127      283 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/__init__.pyi
+-rw-r--r--   0     1001      127       41 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/identifier.py
+-rw-r--r--   0     1001      127      161 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       39 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127      439 2024-04-16 22:48:07.000000 quil-0.9.0rc0/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127      777 2024-04-16 22:48:07.000000 quil-0.9.0rc0/README-py.md
+-rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 quil-0.9.0rc0/PKG-INFO
```

### Comparing `quil-0.8.0/quil-rs/Cargo.toml` & `quil-0.9.0rc0/quil-rs/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "quil-rs"
 description = "Rust tooling for Quil (Quantum Instruction Language)"
-version = "0.24.0"
+version = "0.25.0-rc.0"
 edition = "2021"
 rust-version = "1.70"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rust"
 keywords = ["Quil", "Quantum", "Rigetti"]
 categories = ["parser-implementations", "science", "compilers", "emulators"]
```

### Comparing `quil-0.8.0/quil-rs/CHANGELOG.md` & `quil-0.9.0rc0/quil-rs/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## 0.25.0-rc.0
+
+### Breaking Changes
+
+- Program instruction iteration and serialization is deterministic. (#355)
+
+### Fixes
+
+- Program equality is sensitive to the order of calibration instructions. (#357)
+
+## 0.24.1-rc.0
+
+### Fixes
+
+- Program equality is sensitive to the order of calibration instructions. (#357)
+
 ## 0.24.0
 
 ### Breaking Changes
 
 - CalibrationSet's and Program's will be considered equal if they contain the same set of calibrations, regardless of order. (#352)
 
 ## 0.24.0-rc.0
```

### Comparing `quil-0.8.0/quil-rs/README.md` & `quil-0.9.0rc0/quil-rs/README.md`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/benches/corpus.rs` & `quil-0.9.0rc0/quil-rs/benches/corpus.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/benches/get_frames_for_instruction.rs` & `quil-0.9.0rc0/quil-rs/benches/get_frames_for_instruction.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/benches/parser.rs` & `quil-0.9.0rc0/quil-rs/benches/parser.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/benches/sample-calibrations.quil` & `quil-0.9.0rc0/quil-rs/benches/sample-calibrations.quil`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/benches/scheduled_program_from_program.rs` & `quil-0.9.0rc0/quil-rs/benches/scheduled_program_from_program.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/benches/simplification.rs` & `quil-0.9.0rc0/quil-rs/benches/simplification.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/benches/test_expressions.txt` & `quil-0.9.0rc0/quil-rs/benches/test_expressions.txt`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/examples/generate_test_expressions.rs` & `quil-0.9.0rc0/quil-rs/examples/generate_test_expressions.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/expression/mod.rs` & `quil-0.9.0rc0/quil-rs/src/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/expression/simplification/by_hand.rs` & `quil-0.9.0rc0/quil-rs/src/expression/simplification/by_hand.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/expression/simplification/mod.rs` & `quil-0.9.0rc0/quil-rs/src/expression/simplification/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/hash.rs` & `quil-0.9.0rc0/quil-rs/src/hash.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/calibration.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/circuit.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/classical.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/control_flow.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/declaration.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/frame.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/frame.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-use std::{collections::HashMap, str::FromStr};
+use std::str::FromStr;
 
+use indexmap::IndexMap;
 use nom_locate::LocatedSpan;
 
 use super::{MemoryReference, Qubit, QuotedString, WaveformInvocation};
 use crate::{
     expression::Expression,
     parser::{common::parse_frame_identifier, lex, ParseError},
     program::{disallow_leftover, SyntaxError},
@@ -26,20 +27,20 @@
         match self {
             String(value) => write!(f, "{}", QuotedString(value)).map_err(Into::into),
             Expression(value) => value.write(f, fall_back_to_debug),
         }
     }
 }
 
-pub type FrameAttributes = HashMap<String, AttributeValue>;
+pub type FrameAttributes = IndexMap<String, AttributeValue>;
 
 #[derive(Clone, Debug, PartialEq, Eq)]
 pub struct FrameDefinition {
     pub identifier: FrameIdentifier,
-    pub attributes: HashMap<String, AttributeValue>,
+    pub attributes: FrameAttributes,
 }
 
 impl FrameDefinition {
     pub fn new(identifier: FrameIdentifier, attributes: FrameAttributes) -> Self {
         Self {
             identifier,
             attributes,
```

### Comparing `quil-0.8.0/quil-rs/src/instruction/gate.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/measurement.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/mod.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     PauliSum, PauliTerm,
 };
 pub use self::measurement::Measurement;
 pub use self::pragma::{Include, Pragma, PragmaArgument};
 pub use self::qubit::{Qubit, QubitPlaceholder};
 pub use self::reset::Reset;
 pub use self::timing::{Delay, Fence};
-pub use self::waveform::{Waveform, WaveformDefinition, WaveformInvocation};
+pub use self::waveform::{Waveform, WaveformDefinition, WaveformInvocation, WaveformParameters};
 
 #[derive(Clone, Debug, thiserror::Error, PartialEq, Eq)]
 pub enum ValidationError {
     #[error(transparent)]
     GateError(#[from] GateError),
 }
```

### Comparing `quil-0.8.0/quil-rs/src/instruction/pragma.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/qubit.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/reset.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/timing.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/instruction/waveform.rs` & `quil-0.9.0rc0/quil-rs/src/instruction/waveform.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::collections::HashMap;
+use indexmap::IndexMap;
 
 use crate::{
     expression::Expression,
     quil::{write_join_quil, Quil},
 };
 
 use super::write_parameter_string;
@@ -75,22 +75,24 @@
             snapshot_suffix => description,
         }, {
             assert_snapshot!(waveform_def.to_quil_or_debug())
         })
     }
 }
 
+pub type WaveformParameters = IndexMap<String, Expression>;
+
 #[derive(Clone, Debug, PartialEq, Eq)]
 pub struct WaveformInvocation {
     pub name: String,
-    pub parameters: HashMap<String, Expression>,
+    pub parameters: WaveformParameters,
 }
 
 impl WaveformInvocation {
-    pub fn new(name: String, parameters: HashMap<String, Expression>) -> Self {
+    pub fn new(name: String, parameters: WaveformParameters) -> Self {
         Self { name, parameters }
     }
 }
 
 impl Quil for WaveformInvocation {
     fn write(
         &self,
@@ -120,20 +122,20 @@
         }
         Ok(())
     }
 }
 
 #[cfg(test)]
 mod waveform_invocation_tests {
-    use std::collections::HashMap;
+    use super::WaveformParameters;
 
     use crate::{instruction::WaveformInvocation, quil::Quil};
 
     #[test]
     fn format_no_parameters() {
         let invocation = WaveformInvocation {
             name: "CZ".into(),
-            parameters: HashMap::new(),
+            parameters: WaveformParameters::new(),
         };
         assert_eq!(invocation.to_quil_or_debug(), "CZ".to_string());
     }
 }
```

### Comparing `quil-0.8.0/quil-rs/src/lib.rs` & `quil-0.9.0rc0/quil-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/macros.rs` & `quil-0.9.0rc0/quil-rs/src/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/command.rs` & `quil-0.9.0rc0/quil-rs/src/parser/command.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/common.rs` & `quil-0.9.0rc0/quil-rs/src/parser/common.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-use std::{collections::HashMap, str::FromStr};
+use std::str::FromStr;
 
 use nom::{
     branch::alt,
     combinator::{cut, map, map_res, opt, value},
     multi::{many0, many1, separated_list0, separated_list1},
     sequence::{delimited, pair, preceded, tuple},
 };
 
 use crate::{
     expected_token,
     expression::Expression,
     instruction::{
         ArithmeticOperand, AttributeValue, BinaryOperand, ComparisonOperand, FrameIdentifier,
         GateModifier, MemoryReference, Offset, PauliGate, PauliTerm, Qubit, ScalarType, Sharing,
-        Vector, WaveformInvocation,
+        Vector, WaveformInvocation, WaveformParameters,
     },
     parser::lexer::Operator,
     token,
 };
 
 use crate::parser::{InternalParseError, InternalParserResult};
 
@@ -304,15 +304,15 @@
     let (input, name) = parse_waveform_name(input)?;
     let (input, parameter_tuples) = opt(delimited(
         token!(LParenthesis),
         cut(separated_list0(token!(Comma), parse_named_argument)),
         token!(RParenthesis),
     ))(input)?;
     let parameter_tuples = parameter_tuples.unwrap_or_default();
-    let parameters: HashMap<_, _> = parameter_tuples.into_iter().collect();
+    let parameters: WaveformParameters = parameter_tuples.into_iter().collect();
 
     Ok((input, WaveformInvocation { name, parameters }))
 }
 
 /// Parse a single qubit, which may be an integer (`1`), variable (`%q1`), or identifier (`q1`).
 /// Per the specification, variable-named and identifier-named are valid in different locations,
 /// but this parser is tolerant and accepts both as equivalent.
@@ -472,15 +472,15 @@
 
 #[cfg(test)]
 pub mod tests {
     use crate::{
         expression::{
             Expression, InfixExpression, InfixOperator, PrefixExpression, PrefixOperator,
         },
-        instruction::{MemoryReference, PauliGate, PauliTerm},
+        instruction::{MemoryReference, PauliGate, PauliTerm, WaveformParameters},
         parser::lex,
         real,
     };
 
     use nom_locate::LocatedSpan;
 
     use super::{parse_matrix, parse_pauli_terms, parse_permutation, parse_waveform_invocation};
@@ -562,15 +562,15 @@
                     Expression::Address(MemoryReference {
                         name: "ro".to_owned(),
                         index: 0
                     })
                 )
             ]
             .into_iter()
-            .collect()
+            .collect::<WaveformParameters>()
         )
     }
 
     #[test]
     fn test_parse_matrix() {
         let input = LocatedSpan::new("\n\t1/sqrt(2), 1/sqrt(2)\n\t1/sqrt(2), -1/sqrt(2)");
         let lexed = lex(input).unwrap();
```

### Comparing `quil-0.8.0/quil-rs/src/parser/error/error.rs` & `quil-0.9.0rc0/quil-rs/src/parser/error/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/error/input.rs` & `quil-0.9.0rc0/quil-rs/src/parser/error/input.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/error/internal.rs` & `quil-0.9.0rc0/quil-rs/src/parser/error/internal.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/error/kind.rs` & `quil-0.9.0rc0/quil-rs/src/parser/error/kind.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/error/mod.rs` & `quil-0.9.0rc0/quil-rs/src/parser/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/expression.rs` & `quil-0.9.0rc0/quil-rs/src/parser/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/gate.rs` & `quil-0.9.0rc0/quil-rs/src/parser/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/instruction.rs` & `quil-0.9.0rc0/quil-rs/src/parser/instruction.rs`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,14 @@
         token!(NewLine),
         preceded(token!(Indentation), parse_instruction),
     )(input)
 }
 
 #[cfg(test)]
 mod tests {
-    use std::collections::HashMap;
     use std::str::FromStr;
 
     use nom_locate::LocatedSpan;
     use num_complex::Complex;
 
     use crate::expression::{
         Expression, ExpressionFunction, FunctionCallExpression, InfixExpression, InfixOperator,
@@ -161,15 +160,15 @@
     use crate::instruction::{
         Arithmetic, ArithmeticOperand, ArithmeticOperator, AttributeValue, BinaryLogic,
         BinaryOperand, BinaryOperator, Calibration, Capture, Comparison, ComparisonOperand,
         ComparisonOperator, Convert, FrameDefinition, FrameIdentifier, Gate, GateDefinition,
         GateSpecification, Include, Instruction, Jump, JumpWhen, Label, MemoryReference, Move,
         Pulse, Qubit, RawCapture, Reset, SetFrequency, SetPhase, SetScale, ShiftFrequency,
         ShiftPhase, SwapPhases, Target, UnaryLogic, UnaryOperator, Waveform, WaveformDefinition,
-        WaveformInvocation,
+        WaveformInvocation, WaveformParameters,
     };
     use crate::parser::common::tests::KITCHEN_SINK_QUIL;
     use crate::parser::lexer::lex;
     use crate::quil::Quil;
     use crate::{make_test, real, Program};
 
     use super::parse_instructions;
@@ -468,15 +467,15 @@
                 blocking: true,
                 frame: FrameIdentifier {
                     name: "rx".to_owned(),
                     qubits: vec![Qubit::Fixed(0)]
                 },
                 waveform: WaveformInvocation {
                     name: "my_custom_waveform".to_owned(),
-                    parameters: HashMap::new()
+                    parameters: WaveformParameters::new()
                 },
                 memory_reference: MemoryReference {
                     name: "ro".to_owned(),
                     index: 0
                 }
             }),
             Instruction::RawCapture(RawCapture {
@@ -641,26 +640,26 @@
                 blocking: true,
                 frame: FrameIdentifier {
                     name: "xy".to_owned(),
                     qubits: vec![Qubit::Fixed(0)]
                 },
                 waveform: WaveformInvocation {
                     name: "custom".to_owned(),
-                    parameters: HashMap::new()
+                    parameters: WaveformParameters::new()
                 }
             }),
             Instruction::Pulse(Pulse {
                 blocking: false,
                 frame: FrameIdentifier {
                     name: "xy".to_owned(),
                     qubits: vec![Qubit::Fixed(0)]
                 },
                 waveform: WaveformInvocation {
                     name: "custom".to_owned(),
-                    parameters: HashMap::new()
+                    parameters: WaveformParameters::new()
                 }
             }),
             Instruction::Pulse(Pulse {
                 blocking: true,
                 frame: FrameIdentifier {
                     name: "xy".to_owned(),
                     qubits: vec![Qubit::Fixed(0)]
```

### Comparing `quil-0.8.0/quil-rs/src/parser/lexer/error.rs` & `quil-0.9.0rc0/quil-rs/src/parser/lexer/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/lexer/mod.rs` & `quil-0.9.0rc0/quil-rs/src/parser/lexer/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/lexer/quoted_strings.rs` & `quil-0.9.0rc0/quil-rs/src/parser/lexer/quoted_strings.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/lexer/wrapped_parsers.rs` & `quil-0.9.0rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/macros.rs` & `quil-0.9.0rc0/quil-rs/src/parser/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/mod.rs` & `quil-0.9.0rc0/quil-rs/src/parser/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/parser/token.rs` & `quil-0.9.0rc0/quil-rs/src/parser/token.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/analysis/control_flow_graph.rs` & `quil-0.9.0rc0/quil-rs/src/program/analysis/control_flow_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/analysis/mod.rs` & `quil-0.9.0rc0/quil-rs/src/program/analysis/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/analysis/qubit_graph.rs` & `quil-0.9.0rc0/quil-rs/src/program/analysis/qubit_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap` & `quil-0.9.0rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/analysis/test_programs.rs` & `quil-0.9.0rc0/quil-rs/src/program/analysis/test_programs.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/calibration.rs` & `quil-0.9.0rc0/quil-rs/src/program/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/calibration_set.rs` & `quil-0.9.0rc0/quil-rs/src/program/calibration_set.rs`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,16 @@
 ///
 /// During calibration expansion, Calibrations are matched to instructions using their unique
 /// [`CalibrationSignature`]. This means only one calibration can be matched to a particular
 /// instruction. While the Quil specification doesn't explicitly define the behavior of
 /// signature conflicts, [`CalibrationSet`] takes the liberty of only allowing one calibration
 /// per [`CalibrationSignature`].
 ///
-/// In addition, calibration instructions are global. That is, their order or location in a
-/// program make no semantic difference. This means two program [`CalibrationSet`]s
-/// should be considered equal if they contain the same set of calibrations, regardless of
-/// order.
-///
-/// As a matter of convenience, the insertion order of calibrations is maintained. This
-/// allows for the same set of calibrations to be deterministically serialized to Quil.
-#[derive(Clone, Debug)]
+/// Calibrations maintain insertion order
+#[derive(Clone, Debug, PartialEq)]
 pub struct CalibrationSet<T> {
     // The amount of calibrations in a program tends to be small enough that a Vec is more
     // performant than a typical set.
     // Sets also have trait bounds that `Instruction`s don't meet, which hampers utility.
     data: Vec<T>,
 }
 
@@ -151,34 +145,14 @@
     {
         for value in iter {
             self.replace(value);
         }
     }
 }
 
-impl<T> PartialEq for CalibrationSet<T>
-where
-    T: CalibrationSignature + PartialEq,
-    for<'a> <T as CalibrationSignature>::Signature<'a>: std::hash::Hash + Eq,
-{
-    fn eq(&self, other: &Self) -> bool {
-        let self_map: std::collections::HashMap<T::Signature<'_>, &T> = self
-            .data
-            .iter()
-            .map(|element| (element.signature(), element))
-            .collect();
-        let other_map: std::collections::HashMap<T::Signature<'_>, &T> = other
-            .data
-            .iter()
-            .map(|element| (element.signature(), element))
-            .collect();
-        self_map == other_map
-    }
-}
-
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::instruction::CalibrationSignature;
 
     #[derive(Clone, Debug, PartialEq)]
     struct TestCalibration {
@@ -232,22 +206,22 @@
         let calib = TestCalibration::new("Original", None);
         set.replace(calib.clone());
         assert!(set.remove(&calib.signature()));
         assert!(set.is_empty());
     }
 
     #[test]
-    fn test_equality() {
+    fn test_order_sensitive_equality() {
         let mut set1 = CalibrationSet::new();
         let mut set2 = CalibrationSet::new();
         let calib1 = TestCalibration::new("1", None);
         let calib2 = TestCalibration::new("2", None);
         set1.extend(vec![calib1.clone(), calib2.clone()]);
         set2.extend(vec![calib2, calib1]); // Reverse order
-        assert_eq!(set1, set2); // They should be equal
+        assert_ne!(set1, set2)
     }
 
     #[test]
     fn test_maintains_insert_order() {
         let calibs = vec![
             TestCalibration::new("1", None),
             TestCalibration::new("2", None),
```

### Comparing `quil-0.8.0/quil-rs/src/program/error/leftover.rs` & `quil-0.9.0rc0/quil-rs/src/program/error/leftover.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/error/mod.rs` & `quil-0.9.0rc0/quil-rs/src/program/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/error/result.rs` & `quil-0.9.0rc0/quil-rs/src/program/error/result.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/error/syntax.rs` & `quil-0.9.0rc0/quil-rs/src/program/error/syntax.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/frame.rs` & `quil-0.9.0rc0/quil-rs/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/memory.rs` & `quil-0.9.0rc0/quil-rs/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/mod.rs` & `quil-0.9.0rc0/quil-rs/src/program/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-use std::collections::{BTreeMap, HashMap, HashSet};
+use std::collections::{HashMap, HashSet};
 use std::ops;
 use std::str::FromStr;
 
-use indexmap::IndexSet;
+use indexmap::{IndexMap, IndexSet};
 use ndarray::Array2;
 use nom_locate::LocatedSpan;
 
 use crate::instruction::{
     Arithmetic, ArithmeticOperand, ArithmeticOperator, Declaration, FrameDefinition,
     FrameIdentifier, GateDefinition, GateError, Instruction, Jump, JumpUnless, Label, Matrix,
     MemoryReference, Move, Qubit, QubitPlaceholder, ScalarType, Target, TargetPlaceholder, Vector,
@@ -70,30 +70,30 @@
 /// This contains not only instructions which are executed in turn on the quantum processor, but
 /// also the "headers" used to describe and manipulate those instructions, such as calibrations
 /// and frame definitions.
 #[derive(Clone, Debug, Default, PartialEq)]
 pub struct Program {
     pub calibrations: Calibrations,
     pub frames: FrameSet,
-    pub memory_regions: BTreeMap<String, MemoryRegion>,
-    pub waveforms: BTreeMap<String, Waveform>,
-    pub gate_definitions: BTreeMap<String, GateDefinition>,
+    pub memory_regions: IndexMap<String, MemoryRegion>,
+    pub waveforms: IndexMap<String, Waveform>,
+    pub gate_definitions: IndexMap<String, GateDefinition>,
     instructions: Vec<Instruction>,
     // private field used for caching operations
     used_qubits: HashSet<Qubit>,
 }
 
 impl Program {
     pub fn new() -> Self {
         Program {
             calibrations: Calibrations::default(),
             frames: FrameSet::new(),
-            memory_regions: BTreeMap::new(),
-            waveforms: BTreeMap::new(),
-            gate_definitions: BTreeMap::new(),
+            memory_regions: IndexMap::new(),
+            waveforms: IndexMap::new(),
+            gate_definitions: IndexMap::new(),
             instructions: vec![],
             used_qubits: HashSet::new(),
         }
     }
 
     /// Returns an iterator over immutable references to the instructions that make up the body of the program.
     pub fn body_instructions(&self) -> impl Iterator<Item = &Instruction> {
@@ -1393,29 +1393,118 @@
         let program = Program::from_str(input).unwrap();
 
         // The order of definitions are global in the sense that where they are defined in a
         // program does not matter.
         let is_global_state_instruction = move |i: &Instruction| -> bool {
             matches!(
                 i,
-                Instruction::CalibrationDefinition(_)
-                    | Instruction::MeasureCalibrationDefinition(_)
-                    | Instruction::WaveformDefinition(_)
-                    | Instruction::GateDefinition(_)
+                |Instruction::WaveformDefinition(_)| Instruction::GateDefinition(_)
                     | Instruction::FrameDefinition(_)
             )
         };
         // Create a copy of the program, but insert the "global" instructions in reverse order.
         // Since where these instructions are defined doesn't matter, this should be an
         // equivalent program.
         let mut program2 = program.filter_instructions(|i| !is_global_state_instruction(i));
         let global_instructions: Vec<Instruction> = program
             .filter_instructions(is_global_state_instruction)
             .into_instructions()
             .into_iter()
             .rev()
             .collect();
-        program2.add_instructions(global_instructions);
-
+        program2.add_instructions(global_instructions.clone());
         assert_eq!(program, program2);
+
+        // Create another copy of the program with non-global instructions inserted in reverse order.
+        // This should not be equal to the original program.
+        let mut program3 = Program::from_instructions(
+            program
+                .filter_instructions(|i| !is_global_state_instruction(i))
+                .into_instructions()
+                .into_iter()
+                .rev()
+                .collect(),
+        );
+        program3.add_instructions(global_instructions);
+        assert!(program != program3)
+    }
+
+    #[test]
+    fn test_deterministic_serialization() {
+        let input = "DECLARE foo REAL[1]
+DECLARE bar BIT[1]
+DECLARE baz BIT[1]
+RX(pi) 0
+CNOT 0 1
+DEFCAL I 0:
+\tDELAY 0 1
+\tDELAY 1 1
+DEFCAL I 1:
+\tDELAY 0 1
+\tDELAY 1 2
+DEFCAL I 2:
+\tDELAY 2 1
+\tDELAY 2 3
+DEFCAL MEASURE 0 addr:
+\tRX(pi) 0
+\tCAPTURE 0 \"ro_rx\" custom addr
+DEFCAL MEASURE 1 addr:
+\tRX(pi/2) 1
+\tCAPTURE 1 \"ro_rx\" custom addr
+DEFCAL MEASURE 2 addr:
+\tRX(pi/2) 2
+\tCAPTURE 2 \"ro_rx\" custom addr
+DEFWAVEFORM custom:
+\t1,2
+DEFWAVEFORM custom2:
+\t3,4
+DEFWAVEFORM another1(%a, %b):
+\t%a,%b
+PULSE 0 \"xy\" flat(duration: 1e-6, iq: 2+3i)
+PULSE 0 \"xy\" another1(a: 1e-6, b: 2+3i)
+DEFGATE HADAMARD AS MATRIX:
+\t(1/sqrt(2)),(1/sqrt(2))
+\t(1/sqrt(2)),((-1)/sqrt(2))
+DEFGATE RX(%theta) AS MATRIX:
+\tcos((%theta/2)),((-1i)*sin((%theta/2)))
+\t((-1i)*sin((%theta/2))),cos((%theta/2))
+DEFGATE Name AS PERMUTATION:
+\t1, 0
+DEFCIRCUIT SIMPLE:
+\tX 0
+\tX 1
+DEFGATE BAR AS MATRIX:
+\t0, 1
+\t1, 0
+DEFGATE FOO AS MATRIX:
+\t0, 1
+\t1, 0
+DEFGATE BAZ AS MATRIX:
+\t1, 0
+\t0, 1
+MEASURE 1 bar
+MEASURE 0 foo
+HALT
+DEFCIRCUIT CIRCFOO:
+\tLABEL @FOO_A
+\tJUMP @FOO_A
+DEFFRAME 0 \"xy\":
+\tSAMPLE-RATE: 3000
+DEFFRAME 0 \"xy\":
+\tDIRECTION: \"rx\"
+\tCENTER-FREQUENCY: 1000
+\tHARDWARE-OBJECT: \"some object\"
+\tINITIAL-FREQUENCY: 2000
+\tSAMPLE-RATE: 3000";
+        let program = Program::from_str(input).unwrap();
+        let quil = program.to_quil().unwrap();
+
+        // Asserts that serialization doesn't change on repeated attempts.
+        // 100 is chosen because it should be more than sufficient to reveal an
+        //     issue and it has a negligible impact on execution speed of the test suite.
+        let iterations = 100;
+        for _ in 0..iterations {
+            let new_program = Program::from_str(input).unwrap();
+            assert_eq!(new_program.to_quil().unwrap(), quil);
+        }
     }
 }
```

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/graph.rs` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/graphviz_dot.rs` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/graphviz_dot.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/schedule.rs` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/schedule.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap` & `quil-0.9.0rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap` & `quil-0.9.0rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/program/type_check.rs` & `quil-0.9.0rc0/quil-rs/src/program/type_check.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 //! Type check Quil programs.
 //!
 //! See the [Quil spec](https://quil-lang.github.io/).
+use std::fmt::Debug;
+
+use indexmap::IndexMap;
+use thiserror::Error;
+
 use crate::{
     expression::{Expression, FunctionCallExpression, InfixExpression, PrefixExpression},
     instruction::{
         Arithmetic, ArithmeticOperand, ArithmeticOperator, BinaryLogic, BinaryOperand,
         BinaryOperands, BinaryOperator, Comparison, ComparisonOperand, ComparisonOperator,
         Exchange, Instruction, Load, MemoryReference, Move, ScalarType, SetFrequency, SetPhase,
         SetScale, ShiftFrequency, ShiftPhase, Store, UnaryLogic, UnaryOperator,
     },
     program::MemoryRegion,
     quil::Quil,
     Program,
 };
-use std::collections::BTreeMap;
-use std::fmt::Debug;
-use thiserror::Error;
 
 /// Different types of errors that can occur during type checking.
 #[derive(Debug, Error)]
 pub enum TypeError {
     #[error("In instruction {instruction}: undefined memory reference {reference}.", instruction=.instruction.to_quil_or_debug())]
     UndefinedMemoryReference {
         instruction: Instruction,
@@ -191,15 +193,15 @@
     })
 }
 
 /// In the [Instruction], the given [Expression] should be real-valued.
 fn should_be_real(
     instruction: &Instruction,
     this_expression: &Expression,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     match this_expression {
         Expression::Address(reference) => {
             if let Some(MemoryRegion { size, .. }) = memory_regions.get(&reference.name) {
                 let dt = &size.data_type;
                 if dt == &ScalarType::Real {
                     Ok(())
@@ -236,15 +238,15 @@
 
 /// Type check an [Instruction::Arithmetic].
 fn type_check_arithmetic(
     instruction: &Instruction,
     operator: &ArithmeticOperator,
     destination: &ArithmeticOperand,
     source: &ArithmeticOperand,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     match destination {
         ArithmeticOperand::LiteralInteger(_) | ArithmeticOperand::LiteralReal(_) => {
             operator_operand_mismatch(
                 instruction,
                 "operation",
                 "memory reference",
@@ -300,15 +302,15 @@
 }
 
 /// Type check an [Instruction::Comparison].
 fn type_check_comparison(
     instruction: &Instruction,
     operator: &ComparisonOperator,
     operands: &(MemoryReference, MemoryReference, ComparisonOperand),
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     let (x, y, z) = operands;
     match (memory_regions.get(&x.name), memory_regions.get(&y.name)) {
         (None, _) => undefined_memory_reference(instruction, x),
         (_, None) => undefined_memory_reference(instruction, y),
         (Some(x_region), Some(y_region)) => {
             let (xt, yt) = (&x_region.size.data_type, &y_region.size.data_type);
@@ -342,15 +344,15 @@
 }
 
 /// Type check an [Instruction::BinaryLogic].
 fn type_check_binary_logic(
     instruction: &Instruction,
     operator: &BinaryOperator,
     operands: &BinaryOperands,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     let (x, y) = operands;
     if let Some(x_region) = memory_regions.get(&x.name) {
         let xt = &x_region.size.data_type;
         if xt == &ScalarType::Real {
             operator_operand_mismatch(instruction, operator, "integral", x, xt)
         } else {
@@ -376,15 +378,15 @@
 }
 
 /// Type check an [Instruction::UnaryLogic].
 fn type_check_unary_logic(
     instruction: &Instruction,
     operator: &UnaryOperator,
     operand: &MemoryReference,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     if let Some(MemoryRegion { size, .. }) = memory_regions.get(&operand.name) {
         let dt = &size.data_type;
         match (dt, operator) {
             (ScalarType::Real, UnaryOperator::Not) => {
                 operator_operand_mismatch(instruction, operator, "integral", operand, dt)
             }
@@ -410,15 +412,15 @@
 }
 
 /// Type check an [Instruction::Move].
 fn type_check_move(
     instruction: &Instruction,
     destination: &MemoryReference,
     source: &ArithmeticOperand,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     if let Some(dest_region) = memory_regions.get(&destination.name) {
         let dt = &dest_region.size.data_type;
         match (source, dt) {
             (ArithmeticOperand::LiteralInteger(_), ScalarType::Real) => {
                 data_type_mismatch(instruction, destination, dt, source, "`literal integer`")
             }
@@ -445,15 +447,15 @@
 }
 
 /// Type check an [Instruction::Exchange].
 fn type_check_exchange(
     instruction: &Instruction,
     left: &MemoryReference,
     right: &MemoryReference,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     match (
         memory_regions.get(&left.name),
         memory_regions.get(&right.name),
     ) {
         (None, _) => undefined_memory_reference(instruction, left),
         (_, None) => undefined_memory_reference(instruction, right),
@@ -470,15 +472,15 @@
 
 /// Type check an [Instruction::Load].
 fn type_check_load(
     instruction: &Instruction,
     destination: &MemoryReference,
     source: &str,
     offset: &MemoryReference,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     match (
         memory_regions.get(&destination.name),
         memory_regions.get(source),
         memory_regions.get(&offset.name),
     ) {
         (None, _, _) => undefined_memory_reference(instruction, destination),
@@ -503,15 +505,15 @@
 
 /// type check an [Instruction::Store].
 fn type_check_store(
     instruction: &Instruction,
     destination: &str,
     offset: &MemoryReference,
     source: &ArithmeticOperand,
-    memory_regions: &BTreeMap<String, MemoryRegion>,
+    memory_regions: &IndexMap<String, MemoryRegion>,
 ) -> TypeResult<()> {
     let dest_region =
         memory_regions
             .get(destination)
             .ok_or(TypeError::UndefinedMemoryReference {
                 instruction: instruction.clone(),
                 reference: destination.to_string(),
```

### Comparing `quil-0.8.0/quil-rs/src/quil.rs` & `quil-0.9.0rc0/quil-rs/src/quil.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/reserved.rs` & `quil-0.9.0rc0/quil-rs/src/reserved.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/src/validation/identifier.rs` & `quil-0.9.0rc0/quil-rs/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/calibration_test.rs` & `quil-0.9.0rc0/quil-rs/tests/calibration_test.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/programs/calibration_cz.quil` & `quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz.quil`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/programs/calibration_cz_phase.quil` & `quil-0.9.0rc0/quil-rs/tests/programs/calibration_cz_phase.quil`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/programs/calibration_measure.quil` & `quil-0.9.0rc0/quil-rs/tests/programs/calibration_measure.quil`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/programs/calibration_rx.quil` & `quil-0.9.0rc0/quil-rs/tests/programs/calibration_rx.quil`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/programs/calibration_xy.quil` & `quil-0.9.0rc0/quil-rs/tests/programs/calibration_xy.quil`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap` & `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap` & `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap` & `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap` & `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap` & `quil-0.9.0rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/Cargo.toml` & `quil-0.9.0rc0/quil-py/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "quil-py"
 description = "Python bindings for quil-rs"
-version = "0.8.0"
+version = "0.9.0-rc.0"
 edition = "2021"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rs"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "parsers", "science", "emulators"]
 readme = "./README.md"
 
@@ -18,17 +18,17 @@
 #
 # Downstream Rust code (including code in `bin/`, `examples/`, and `tests/`) will not be able
 # to `use quil;` unless the "lib" and "rlib" crate type is also included:
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
 ndarray.workspace = true
-quil-rs = { path = "../quil-rs", version = "0.24.0" }
+quil-rs = { path = "../quil-rs", version = "0.25.0-rc.0" }
 strum.workspace = true
 # pyo3 dependencies should be updated together
 numpy = "0.20.0"
 pyo3 = { version = "0.20.3", features = ["indexmap"] }
-rigetti-pyo3 = "0.3.1"
+rigetti-pyo3 = {version = "0.3.4", features = ["indexmap"]}
 indexmap.workspace = true
 
 [build-dependencies]
 pyo3-build-config = "0.20.0"
```

### Comparing `quil-0.8.0/quil-py/CHANGELOG.md` & `quil-0.9.0rc0/quil-py/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## 0.9.0-rc.0
+
+### Breaking Changes
+
+- Program instruction iteration and serialization is deterministic. (#355)
+
+### Fixes
+
+- Program equality is sensitive to the order of calibration instructions. (#357)
+
+## 0.8.1-rc.0
+
+### Fixes
+
+- Program equality is sensitive to the order of calibration instructions. (#357)
+
 ## 0.8.0
 
 ### Breaking Changes
 
 - CalibrationSet's and Program's will be considered equal if they contain the same set of calibrations, regardless of order. (#352)
 
 ## 0.8.0-rc.0
```

### Comparing `quil-0.8.0/quil-py/Makefile.toml` & `quil-0.9.0rc0/quil-py/Makefile.toml`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/README-py.md` & `quil-0.9.0rc0/quil-py/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/out/quil/quil.html` & `quil-0.9.0rc0/quil-py/out/quil/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/out/quil.html` & `quil-0.9.0rc0/quil-py/out/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/out/search.js` & `quil-0.9.0rc0/quil-py/out/search.js`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/poetry.lock` & `quil-0.9.0rc0/quil-py/poetry.lock`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/quil/expression/__init__.pyi` & `quil-0.9.0rc0/quil-py/quil/expression/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/quil/instructions/__init__.pyi` & `quil-0.9.0rc0/quil-py/quil/instructions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/quil/program/__init__.pyi` & `quil-0.9.0rc0/quil-py/quil/program/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/quil.html` & `quil-0.9.0rc0/quil-py/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/expression.rs` & `quil-0.9.0rc0/quil-py/src/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/calibration.rs` & `quil-0.9.0rc0/quil-py/src/instruction/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/circuit.rs` & `quil-0.9.0rc0/quil-py/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/classical.rs` & `quil-0.9.0rc0/quil-py/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/control_flow.rs` & `quil-0.9.0rc0/quil-py/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/declaration.rs` & `quil-0.9.0rc0/quil-py/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/frame.rs` & `quil-0.9.0rc0/quil-py/src/instruction/frame.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-use std::collections::HashMap;
 use std::hash::Hash;
 
+use indexmap::IndexMap;
+
 use quil_rs::{
     expression::Expression,
     instruction::{
         AttributeValue, Capture, FrameAttributes, FrameDefinition, FrameIdentifier,
         MemoryReference, Pulse, Qubit, RawCapture, SetFrequency, SetPhase, SetScale,
         ShiftFrequency, ShiftPhase, SwapPhases, WaveformInvocation,
     },
@@ -34,22 +35,22 @@
     }
 }
 impl_repr!(PyAttributeValue);
 impl_to_quil!(PyAttributeValue);
 impl_hash!(PyAttributeValue);
 impl_eq!(PyAttributeValue);
 
-pub type PyFrameAttributes = HashMap<String, PyAttributeValue>;
+pub type PyFrameAttributes = IndexMap<String, PyAttributeValue>;
 
 py_wrap_data_struct! {
     #[derive(Debug, PartialEq, Eq)]
     #[pyo3(subclass)]
     PyFrameDefinition(FrameDefinition) as "FrameDefinition" {
         identifier: FrameIdentifier => PyFrameIdentifier,
-        attributes: HashMap<String, AttributeValue> => PyFrameAttributes
+        attributes: FrameAttributes => PyFrameAttributes
     }
 }
 impl_repr!(PyFrameDefinition);
 impl_to_quil!(PyFrameDefinition);
 impl_copy_for_instruction!(PyFrameDefinition);
 impl_eq!(PyFrameDefinition);
```

### Comparing `quil-0.8.0/quil-py/src/instruction/gate.rs` & `quil-0.9.0rc0/quil-py/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/measurement.rs` & `quil-0.9.0rc0/quil-py/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/mod.rs` & `quil-0.9.0rc0/quil-py/src/instruction/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/pragma.rs` & `quil-0.9.0rc0/quil-py/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/qubit.rs` & `quil-0.9.0rc0/quil-py/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/reset.rs` & `quil-0.9.0rc0/quil-py/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/timing.rs` & `quil-0.9.0rc0/quil-py/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/instruction/waveform.rs` & `quil-0.9.0rc0/quil-py/src/instruction/waveform.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-use std::collections::HashMap;
+use indexmap::IndexMap;
 
 use quil_rs::{
     expression::Expression,
-    instruction::{Waveform, WaveformDefinition, WaveformInvocation},
+    instruction::{Waveform, WaveformDefinition, WaveformInvocation, WaveformParameters},
 };
 
 use rigetti_pyo3::{
     impl_hash, impl_repr, py_wrap_data_struct,
     pyo3::{pymethods, types::PyString, Py, PyResult, Python},
     PyTryFrom,
 };
@@ -61,33 +61,31 @@
         Ok(Self(WaveformDefinition::new(
             name,
             Waveform::py_try_from(py, &definition)?,
         )))
     }
 }
 
+pub type PyWaveformParameters = IndexMap<String, PyExpression>;
+
 py_wrap_data_struct! {
     #[derive(Debug, PartialEq, Eq)]
     #[pyo3(subclass)]
     PyWaveformInvocation(WaveformInvocation) as "WaveformInvocation" {
         name: String => Py<PyString>,
-        parameters: HashMap<String, Expression> => HashMap<String, PyExpression>
+        parameters: WaveformParameters => PyWaveformParameters
     }
 }
 impl_repr!(PyWaveformInvocation);
 impl_to_quil!(PyWaveformInvocation);
 impl_eq!(PyWaveformInvocation);
 
 #[pymethods]
 impl PyWaveformInvocation {
     #[new]
-    pub fn new(
-        py: Python<'_>,
-        name: String,
-        parameters: HashMap<String, PyExpression>,
-    ) -> PyResult<Self> {
+    pub fn new(py: Python<'_>, name: String, parameters: PyWaveformParameters) -> PyResult<Self> {
         Ok(Self(WaveformInvocation::new(
             name,
-            HashMap::<String, Expression>::py_try_from(py, &parameters)?,
+            WaveformParameters::py_try_from(py, &parameters)?,
         )))
     }
 }
```

### Comparing `quil-0.8.0/quil-py/src/lib.rs` & `quil-0.9.0rc0/quil-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/program/analysis.rs` & `quil-0.9.0rc0/quil-py/src/program/analysis.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/program/calibration.rs` & `quil-0.9.0rc0/quil-py/src/program/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/program/frame.rs` & `quil-0.9.0rc0/quil-py/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/program/memory.rs` & `quil-0.9.0rc0/quil-py/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/program/mod.rs` & `quil-0.9.0rc0/quil-py/src/program/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use std::{
-    collections::{BTreeMap, HashMap, HashSet},
+    collections::{HashMap, HashSet},
     str::FromStr,
 };
 
+use indexmap::IndexMap;
 use numpy::{PyArray2, ToPyArray};
 use quil_rs::{
     instruction::{Instruction, QubitPlaceholder, TargetPlaceholder, Waveform},
     program::{
         analysis::{ControlFlowGraph, ControlFlowGraphOwned},
         Calibrations, FrameSet, MemoryRegion,
     },
@@ -110,25 +111,25 @@
     ) -> PyResult<()> {
         let program = self.as_inner_mut();
         program.calibrations = Calibrations::py_try_from(py, &calibrations)?;
         Ok(())
     }
 
     #[getter]
-    pub fn waveforms(&self, py: Python<'_>) -> PyResult<BTreeMap<String, PyWaveform>> {
+    pub fn waveforms(&self, py: Python<'_>) -> PyResult<IndexMap<String, PyWaveform>> {
         self.as_inner().waveforms.to_python(py)
     }
 
     #[setter]
     pub fn set_waveforms(
         &mut self,
         py: Python<'_>,
-        waveforms: BTreeMap<String, PyWaveform>,
+        waveforms: IndexMap<String, PyWaveform>,
     ) -> PyResult<()> {
-        self.as_inner_mut().waveforms = BTreeMap::<String, Waveform>::py_try_from(py, &waveforms)?;
+        self.as_inner_mut().waveforms = IndexMap::<String, Waveform>::py_try_from(py, &waveforms)?;
         Ok(())
     }
 
     #[getter]
     pub fn frames(&self, py: Python<'_>) -> PyResult<PyFrameSet> {
         self.as_inner().frames.to_python(py)
     }
@@ -136,30 +137,30 @@
     #[setter]
     pub fn set_frames(&mut self, py: Python<'_>, frames: PyFrameSet) -> PyResult<()> {
         self.as_inner_mut().frames = FrameSet::py_try_from(py, &frames)?;
         Ok(())
     }
 
     #[getter]
-    pub fn memory_regions(&self, py: Python<'_>) -> PyResult<BTreeMap<String, PyMemoryRegion>> {
+    pub fn memory_regions(&self, py: Python<'_>) -> PyResult<IndexMap<String, PyMemoryRegion>> {
         self.as_inner()
             .memory_regions
             .iter()
             .map(|(name, memory_region)| Ok((name.to_python(py)?, memory_region.to_python(py)?)))
             .collect()
     }
 
     #[setter]
     pub fn set_memory_regions(
         &mut self,
         py: Python<'_>,
-        memory_regions: BTreeMap<String, PyMemoryRegion>,
+        memory_regions: IndexMap<String, PyMemoryRegion>,
     ) -> PyResult<()> {
         self.as_inner_mut().memory_regions =
-            BTreeMap::<String, MemoryRegion>::py_try_from(py, &memory_regions)?;
+            IndexMap::<String, MemoryRegion>::py_try_from(py, &memory_regions)?;
         Ok(())
     }
 
     #[getter]
     // TODO: Should this filtering move to Program? Should we assume memory_regions will always make up all
     // declarations and simplify this?
     pub fn declarations(&self, py: Python<'_>) -> PyResult<HashMap<String, PyDeclaration>> {
@@ -171,24 +172,24 @@
                 _ => None,
             })
             .map(|declaration| Ok((declaration.name.clone(), declaration.to_python(py)?)))
             .collect()
     }
 
     #[getter]
-    pub fn gate_definitions(&self, py: Python<'_>) -> PyResult<BTreeMap<String, PyGateDefinition>> {
+    pub fn gate_definitions(&self, py: Python<'_>) -> PyResult<IndexMap<String, PyGateDefinition>> {
         self.as_inner()
             .gate_definitions
             .iter()
             .map(|(name, gate_def)| Ok((name.to_python(py)?, gate_def.to_python(py)?)))
             .collect()
     }
 
     #[setter]
-    pub fn set_gate_definitions(&mut self, definitions: BTreeMap<String, PyGateDefinition>) {
+    pub fn set_gate_definitions(&mut self, definitions: IndexMap<String, PyGateDefinition>) {
         self.as_inner_mut().gate_definitions = definitions
             .into_iter()
             .map(|(name, gate_def)| (name, gate_def.into_inner()))
             .collect();
     }
 
     pub fn dagger(&self) -> PyResult<Self> {
```

### Comparing `quil-0.8.0/quil-py/src/program/scheduling.rs` & `quil-0.9.0rc0/quil-py/src/program/scheduling.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/src/validation/identifier.rs` & `quil-0.9.0rc0/quil-py/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/test/instructions/test_copy.py` & `quil-0.9.0rc0/quil-py/test/instructions/test_copy.py`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/test/program/test_program.py` & `quil-0.9.0rc0/quil-py/test/program/test_program.py`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil-py/test/test_eq.py` & `quil-0.9.0rc0/quil-py/test/test_eq.py`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/Cargo.lock` & `quil-0.9.0rc0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -315,17 +315,20 @@
 checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "deranged"
-version = "0.3.7"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7684a49fb1af197853ef7b2ee694bc1f5b4179556f1e5710e1760c5db6f5e929"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
+dependencies = [
+ "powerfmt",
+]
 
 [[package]]
 name = "dot-writer"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d1b11bd5e7e98406c6ff39fbc94d6e910a489b978ce7f17c19fce91a1195b7a"
 
@@ -554,17 +557,17 @@
  "lazy_static",
  "linked-hash-map",
  "similar",
 ]
 
 [[package]]
 name = "inventory"
-version = "0.3.11"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a53088c87cf71c9d4f3372a2cb9eea1e7b8a0b1bf8b7f7d23fe5b76dbb07e63b"
+checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
 [[package]]
 name = "is-terminal"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
@@ -797,14 +800,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
@@ -939,14 +948,20 @@
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
+name = "powerfmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
@@ -1067,38 +1082,38 @@
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quil-cli"
-version = "0.1.0"
+version = "0.2.0-rc.1"
 dependencies = [
  "anyhow",
  "clap",
  "quil-rs",
 ]
 
 [[package]]
 name = "quil-py"
-version = "0.8.0"
+version = "0.9.0-rc.0"
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
-version = "0.24.0"
+version = "0.25.0-rc.0"
 dependencies = [
  "approx",
  "clap",
  "criterion",
  "dot-writer",
  "indexmap",
  "insta",
@@ -1253,18 +1268,19 @@
 name = "relative-path"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bf2521270932c3c7bed1a59151222bd7643c79310f2916f01925e1e16255698"
 
 [[package]]
 name = "rigetti-pyo3"
-version = "0.3.1"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff977cba40f2cadf214226cf51c9729a4f5730a5413f901246eed78cb6e795c9"
+checksum = "402e7e159c1a8b5fcd0a2bb7c9b6d50b25f9380a0ecb83930c1e907e3a9737db"
 dependencies = [
+ "indexmap",
  "num-complex",
  "num-traits",
  "paste",
  "pyo3",
  "time",
 ]
 
@@ -1368,26 +1384,26 @@
 name = "semver"
 version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.183"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32ac8da02677876d532745a130fc9d8e6edfa81a269b107c5b00829b91d8eb3c"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.183"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aafe972d60b0b9bee71a91b92fee2d4fb3c9d7e8f6b179aa99f27203d99a4816"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2 1.0.78",
  "quote 1.0.35",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -1515,28 +1531,30 @@
  "proc-macro2 1.0.78",
  "quote 1.0.35",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.25"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fdd63d58b18d663fbdf70e049f00a22c8e42be082203be7f26589213cd75ea"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
+ "num-conv",
+ "powerfmt",
  "serde",
  "time-core",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
```

### Comparing `quil-0.8.0/pyproject.toml` & `quil-0.9.0rc0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   "Operating System :: OS Independent",
 ]
 
 # PEP 621 specifies the [project] table as the source for project metadata. However, Poetry only supports [tool.poetry]
 # We can remove this table once this issue is resolved: https://github.com/python-poetry/poetry/issues/3332
 [tool.poetry]
 name = "quil"
-version = "0.8.0"
+version = "0.9.0-rc.0"
 description = "A Python package for building and parsing Quil programs."
 readme = "README-py.md"
 authors = ["Rigetti Computing <softapps@rigetti.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.21"
```

### Comparing `quil-0.8.0/quil/instructions/__init__.pyi` & `quil-0.9.0rc0/quil/instructions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil/program/__init__.pyi` & `quil-0.9.0rc0/quil/program/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/quil/expression/__init__.pyi` & `quil-0.9.0rc0/quil/expression/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/README-py.md` & `quil-0.9.0rc0/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.8.0/PKG-INFO` & `quil-0.9.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quil
-Version: 0.8.0
+Version: 0.9.0rc0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Summary: A Python package for building and parsing Quil programs.
```

