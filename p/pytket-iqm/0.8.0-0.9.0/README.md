# Comparing `tmp/pytket_iqm-0.8.0-py3-none-any.whl.zip` & `tmp/pytket_iqm-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15065 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      895 b- defN 23-Oct-17 10:51 pytket/extensions/iqm/__init__.py
--rw-rw-rw-  2.0 fat       68 b- defN 23-Oct-17 10:52 pytket/extensions/iqm/_metadata.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-17 10:51 pytket/extensions/iqm/py.typed
--rw-rw-rw-  2.0 fat      708 b- defN 23-Oct-17 10:51 pytket/extensions/iqm/backends/__init__.py
--rw-rw-rw-  2.0 fat     1808 b- defN 23-Oct-17 10:51 pytket/extensions/iqm/backends/config.py
--rw-rw-rw-  2.0 fat    14948 b- defN 23-Oct-17 10:51 pytket/extensions/iqm/backends/iqm.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Oct-17 10:52 pytket_iqm-0.8.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5837 b- defN 23-Oct-17 10:52 pytket_iqm-0.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-17 10:52 pytket_iqm-0.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Oct-17 10:52 pytket_iqm-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      953 b- defN 23-Oct-17 10:52 pytket_iqm-0.8.0.dist-info/RECORD
-11 files, 36874 bytes uncompressed, 13427 bytes compressed:  63.6%
+Zip file size: 14963 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      874 b- defN 23-Nov-24 09:40 pytket/extensions/iqm/__init__.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Nov-24 09:41 pytket/extensions/iqm/_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Nov-24 09:40 pytket/extensions/iqm/py.typed
+-rw-r--r--  2.0 unx      690 b- defN 23-Nov-24 09:40 pytket/extensions/iqm/backends/__init__.py
+-rw-r--r--  2.0 unx     1752 b- defN 23-Nov-24 09:40 pytket/extensions/iqm/backends/config.py
+-rw-r--r--  2.0 unx    14549 b- defN 23-Nov-24 09:40 pytket/extensions/iqm/backends/iqm.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Nov-24 09:41 pytket_iqm-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5689 b- defN 23-Nov-24 09:41 pytket_iqm-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Nov-24 09:41 pytket_iqm-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Nov-24 09:41 pytket_iqm-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      953 b- defN 23-Nov-24 09:41 pytket_iqm-0.9.0.dist-info/RECORD
+11 files, 36029 bytes uncompressed, 13325 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pytket/extensions/iqm/backends/config.py
 Comment: 
 
 Filename: pytket/extensions/iqm/backends/iqm.py
 Comment: 
 
-Filename: pytket_iqm-0.8.0.dist-info/LICENSE
+Filename: pytket_iqm-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_iqm-0.8.0.dist-info/METADATA
+Filename: pytket_iqm-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_iqm-0.8.0.dist-info/WHEEL
+Filename: pytket_iqm-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_iqm-0.8.0.dist-info/top_level.txt
+Filename: pytket_iqm-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_iqm-0.8.0.dist-info/RECORD
+Filename: pytket_iqm-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/iqm/__init__.py

 * *Ordering differences only*

```diff
@@ -1,21 +1,21 @@
-# Copyright 2020-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""Backends for processing pytket circuits with IQM devices
-"""
-
-# _metadata.py is copied to the folder after installation.
-from ._metadata import __extension_version__, __extension_name__
-from .backends import IQMBackend
-from .backends.config import IQMConfig, set_iqm_config
+# Copyright 2020-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Backends for processing pytket circuits with IQM devices
+"""
+
+# _metadata.py is copied to the folder after installation.
+from ._metadata import __extension_version__, __extension_name__
+from .backends import IQMBackend
+from .backends.config import IQMConfig, set_iqm_config
```

## pytket/extensions/iqm/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.8.0"
-__extension_name__ = "pytket-iqm"
+__extension_version__ = "0.9.0"
+__extension_name__ = "pytket-iqm"
```

## pytket/extensions/iqm/backends/__init__.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-# Copyright 2020-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""Backends for processing pytket circuits with IQM devices
-"""
-
-from .iqm import IQMBackend
+# Copyright 2020-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Backends for processing pytket circuits with IQM devices
+"""
+
+from .iqm import IQMBackend
```

## pytket/extensions/iqm/backends/config.py

 * *Ordering differences only*

```diff
@@ -1,56 +1,56 @@
-# Copyright 2020-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""IQM config."""
-
-from typing import Any, Dict, Optional, Type, ClassVar
-from dataclasses import dataclass
-from pytket.config import PytketExtConfig
-
-
-@dataclass
-class IQMConfig(PytketExtConfig):
-    """Holds config parameters for pytket-iqm."""
-
-    ext_dict_key: ClassVar[str] = "iqm"
-
-    auth_server_url: Optional[str]
-    username: Optional[str]
-    password: Optional[str]
-
-    @classmethod
-    def from_extension_dict(
-        cls: Type["IQMConfig"], ext_dict: Dict[str, Any]
-    ) -> "IQMConfig":
-        return cls(
-            ext_dict.get("auth_server_url"),
-            ext_dict.get("username"),
-            ext_dict.get("password"),
-        )
-
-
-def set_iqm_config(
-    auth_server_url: Optional[str] = None,
-    username: Optional[str] = None,
-    password: Optional[str] = None,
-) -> None:
-    """Set default value for IQM API token."""
-    config = IQMConfig.from_default_config_file()
-    if auth_server_url is not None:
-        config.auth_server_url = auth_server_url
-    if username is not None:
-        config.username = username
-    if password is not None:
-        config.password = password
-    config.update_default_config_file()
+# Copyright 2020-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""IQM config."""
+
+from typing import Any, Dict, Optional, Type, ClassVar
+from dataclasses import dataclass
+from pytket.config import PytketExtConfig
+
+
+@dataclass
+class IQMConfig(PytketExtConfig):
+    """Holds config parameters for pytket-iqm."""
+
+    ext_dict_key: ClassVar[str] = "iqm"
+
+    auth_server_url: Optional[str]
+    username: Optional[str]
+    password: Optional[str]
+
+    @classmethod
+    def from_extension_dict(
+        cls: Type["IQMConfig"], ext_dict: Dict[str, Any]
+    ) -> "IQMConfig":
+        return cls(
+            ext_dict.get("auth_server_url"),
+            ext_dict.get("username"),
+            ext_dict.get("password"),
+        )
+
+
+def set_iqm_config(
+    auth_server_url: Optional[str] = None,
+    username: Optional[str] = None,
+    password: Optional[str] = None,
+) -> None:
+    """Set default value for IQM API token."""
+    config = IQMConfig.from_default_config_file()
+    if auth_server_url is not None:
+        config.auth_server_url = auth_server_url
+    if username is not None:
+        config.username = username
+    if password is not None:
+        config.password = password
+    config.update_default_config_file()
```

## pytket/extensions/iqm/backends/iqm.py

 * *Ordering differences only*

```diff
@@ -1,399 +1,399 @@
-# Copyright 2020-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json
-import os
-from typing import cast, Dict, List, Optional, Sequence, Tuple, Union
-from uuid import UUID
-from iqm.iqm_client.iqm_client import Circuit as IQMCircuit
-from iqm.iqm_client.iqm_client import Instruction, IQMClient, Metadata, Status
-import numpy as np
-from pytket.backends import Backend, CircuitStatus, ResultHandle, StatusEnum
-from pytket.backends.backend import KwargTypes
-from pytket.backends.backend_exceptions import CircuitNotRunError
-from pytket.backends.backendinfo import BackendInfo
-from pytket.backends.backendresult import BackendResult
-from pytket.backends.resulthandle import _ResultIdTuple
-from pytket.circuit import Circuit, Node, OpType
-from pytket.extensions.iqm._metadata import __extension_version__
-from pytket.passes import (
-    BasePass,
-    SequencePass,
-    SynthesiseTket,
-    FullPeepholeOptimise,
-    FlattenRegisters,
-    RebaseCustom,
-    DecomposeBoxes,
-    RemoveRedundancies,
-    DefaultMappingPass,
-    DelayMeasures,
-    SimplifyInitial,
-)
-from pytket.predicates import (
-    ConnectivityPredicate,
-    GateSetPredicate,
-    NoClassicalControlPredicate,
-    NoFastFeedforwardPredicate,
-    NoBarriersPredicate,
-    NoMidMeasurePredicate,
-    NoSymbolsPredicate,
-    Predicate,
-)
-from pytket.architecture import Architecture
-from pytket.utils import prepare_circuit
-from pytket.utils.outcomearray import OutcomeArray
-from .config import IQMConfig
-
-# Mapping of natively supported instructions' names to members of Pytket OpType
-_IQM_PYTKET_OP_MAP = {
-    "phased_rx": OpType.PhasedX,
-    "cz": OpType.CZ,
-    "measurement": OpType.Measure,
-    "barrier": OpType.Barrier,
-}
-
-
-class IqmAuthenticationError(Exception):
-    """Raised when there is no IQM access credentials available."""
-
-    def __init__(self) -> None:
-        super().__init__("No IQM access credentials provided or found in config file.")
-
-
-class IQMBackend(Backend):
-    """
-    Interface to an IQM device or simulator.
-    """
-
-    _supports_shots = True
-    _supports_counts = True
-    _supports_contextual_optimisation = True
-    _persistent_handles = True
-
-    def __init__(
-        self,
-        url: str,
-        arch: Optional[List[List[str]]] = None,
-        auth_server_url: Optional[str] = None,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-    ):
-        """
-        Construct a new IQM backend.
-
-        Requires _either_ a valid auth server URL, username and password, _or_ a tokens
-        file.
-
-        Auth server URL, username and password can either be provided as parameters or
-        set in config using :py:meth:`pytket.extensions.iqm.set_iqm_config`.
-
-        Path to the tokens file is read from the environmment variable
-        ``IQM_TOKENS_FILE``. If set, this overrides any other credentials provided as
-        arguments.
-
-        :param url: base URL for requests
-        :param arch: Optional list of couplings between the qubits defined, if
-        not set the default value from the server is used.
-        :param auth_server_url: base URL of authentication server
-        :param username: IQM username
-        :param password: IQM password
-        """
-        super().__init__()
-        self._url = url
-        config = IQMConfig.from_default_config_file()
-
-        if auth_server_url is None:
-            auth_server_url = config.auth_server_url
-        tokens_file = os.getenv("IQM_TOKENS_FILE")
-        if username is None:
-            username = config.username
-        if password is None:
-            password = config.password
-        if (username is None or password is None) and tokens_file is None:
-            raise IqmAuthenticationError()
-
-        if tokens_file is None:
-            self._client = IQMClient(
-                self._url,
-                auth_server_url=auth_server_url,
-                username=username,
-                password=password,
-            )
-        else:
-            self._client = IQMClient(self._url, tokens_file=tokens_file)
-        _iqmqa = self._client.get_quantum_architecture()
-        self._operations = [_IQM_PYTKET_OP_MAP[op] for op in _iqmqa.operations]
-        self._qubits = [_as_node(qb) for qb in _iqmqa.qubits]
-        self._n_qubits = len(self._qubits)
-        if arch is None:
-            arch = _iqmqa.qubit_connectivity
-        coupling = [(_as_node(a), _as_node(b)) for (a, b) in arch]
-        if any(qb not in self._qubits for couple in coupling for qb in couple):
-            raise ValueError("Architecture contains qubits not in device")
-        self._arch = Architecture(coupling)
-        self._backendinfo = BackendInfo(
-            name=type(self).__name__,
-            device_name=_iqmqa.name,
-            version=__extension_version__,
-            architecture=self._arch,
-            gate_set=set(self._operations),
-        )
-
-    @property
-    def backend_info(self) -> BackendInfo:
-        return self._backendinfo
-
-    @property
-    def required_predicates(self) -> List[Predicate]:
-        return [
-            NoClassicalControlPredicate(),
-            NoFastFeedforwardPredicate(),
-            NoBarriersPredicate(),
-            NoMidMeasurePredicate(),
-            NoSymbolsPredicate(),
-            GateSetPredicate(set(self._operations)),
-            ConnectivityPredicate(self._arch),
-        ]
-
-    def rebase_pass(self) -> BasePass:
-        return _iqm_rebase()
-
-    def default_compilation_pass(self, optimisation_level: int = 1) -> BasePass:
-        assert optimisation_level in range(3)
-        passes = [DecomposeBoxes(), FlattenRegisters()]
-        if optimisation_level == 0:
-            passes.append(self.rebase_pass())  # to satisfy MaxTwoQubitGatesPredicate
-        elif optimisation_level == 1:
-            passes.append(SynthesiseTket())
-        elif optimisation_level == 2:
-            passes.append(FullPeepholeOptimise())
-        passes.append(DefaultMappingPass(self._arch))
-        passes.append(DelayMeasures())
-        passes.append(self.rebase_pass())
-        passes.append(RemoveRedundancies())
-        return SequencePass(passes)
-
-    @property
-    def _result_id_type(self) -> _ResultIdTuple:
-        return (bytes, str)
-
-    def process_circuits(
-        self,
-        circuits: Sequence[Circuit],
-        n_shots: Union[None, int, Sequence[Optional[int]]] = None,
-        valid_check: bool = True,
-        **kwargs: KwargTypes,
-    ) -> List[ResultHandle]:
-        """
-        See :py:meth:`pytket.backends.Backend.process_circuits`.
-
-        Supported `kwargs`:
-        - `postprocess`: apply end-of-circuit simplifications and classical
-          postprocessing to improve fidelity of results (bool, default False)
-        - `simplify_initial`: apply the pytket ``SimplifyInitial`` pass to improve
-          fidelity of results assuming all qubits initialized to zero (bool, default
-          False)
-        """
-        circuits = list(circuits)
-        n_shots_list = Backend._get_n_shots_as_list(
-            n_shots,
-            len(circuits),
-            optional=False,
-        )
-
-        if valid_check:
-            self._check_all_circuits(circuits)
-
-        postprocess = kwargs.get("postprocess", False)
-        simplify_initial = kwargs.get("postprocess", False)
-
-        handles = []
-        for i, (c, n_shots) in enumerate(zip(circuits, n_shots_list)):
-            if postprocess:
-                c0, ppcirc = prepare_circuit(c, allow_classical=False, xcirc=_xcirc)
-                ppcirc_rep = ppcirc.to_dict()
-            else:
-                c0, ppcirc_rep = c, None
-            if simplify_initial:
-                SimplifyInitial(
-                    allow_classical=False, create_all_qubits=True, xcirc=_xcirc
-                ).apply(c0)
-            instrs = _translate_iqm(c0)
-            qm = {str(qb): _as_name(cast(Node, qb)) for qb in c.qubits}
-            iqmc = IQMCircuit(
-                name=c.name if c.name else f"circuit_{i}",
-                instructions=instrs,
-                metadata=None,
-            )
-            run_id = self._client.submit_circuits(
-                [iqmc], qubit_mapping=qm, shots=n_shots
-            )
-            handles.append(ResultHandle(run_id.bytes, json.dumps(ppcirc_rep)))
-        for handle in handles:
-            self._cache[handle] = dict()
-        return handles
-
-    def _update_cache_result(
-        self, handle: ResultHandle, result_dict: Dict[str, BackendResult]
-    ) -> None:
-        if handle in self._cache:
-            self._cache[handle].update(result_dict)
-        else:
-            self._cache[handle] = result_dict
-
-    def circuit_status(self, handle: ResultHandle) -> CircuitStatus:
-        self._check_handle_type(handle)
-        run_id = UUID(bytes=cast(bytes, handle[0]))
-        run_result = self._client.get_run(run_id)
-        status = run_result.status
-        if status == Status.PENDING_EXECUTION:
-            return CircuitStatus(StatusEnum.SUBMITTED)
-        elif status == Status.READY:
-            measurements = cast(dict, run_result.measurements)[0]
-            shots = OutcomeArray.from_readouts(
-                np.array(
-                    [[r[0] for r in rlist] for cbstr, rlist in measurements.items()],
-                    dtype=int,
-                )
-                .transpose()
-                .tolist()
-            )
-            ppcirc_rep = json.loads(cast(str, handle[1]))
-            ppcirc = Circuit.from_dict(ppcirc_rep) if ppcirc_rep is not None else None
-            self._update_cache_result(
-                handle, {"result": BackendResult(shots=shots, ppcirc=ppcirc)}
-            )
-            return CircuitStatus(StatusEnum.COMPLETED)
-        else:
-            assert status == Status.FAILED
-            return CircuitStatus(StatusEnum.ERROR, cast(str, run_result.message))
-
-    def get_result(self, handle: ResultHandle, **kwargs: KwargTypes) -> BackendResult:
-        """
-        See :py:meth:`pytket.backends.Backend.get_result`.
-        Supported kwargs: `timeout` (default 900).
-        """
-        try:
-            return super().get_result(handle)
-        except CircuitNotRunError:
-            timeout = kwargs.get("timeout", 900)
-            # Wait for job to finish; result will then be in the cache.
-            run_id = UUID(bytes=cast(bytes, handle[0]))
-            self._client.wait_for_results(run_id, timeout_secs=cast(float, timeout))
-            circuit_status = self.circuit_status(handle)
-            if circuit_status.status is StatusEnum.COMPLETED:
-                return cast(BackendResult, self._cache[handle]["result"])
-            else:
-                assert circuit_status.status is StatusEnum.ERROR
-                raise RuntimeError(circuit_status.message)
-
-    def get_metadata(self, handle: ResultHandle, **kwargs: KwargTypes) -> Metadata:
-        """Return the metadata corresponding to the handle.
-
-        Use keyword arguments to specify parameters to be used in retrieving
-        the metadata.
-
-        * `timeout`: maximum time to wait for remote job to finish
-
-        Example usage:
-            n_shots = 100
-            backend.run_circuit(circuit, n_shots=n_shots, timeout=30)
-            handle = backend.process_circuits([circuit], n_shots=n_shots)[0]
-            result = backend.get_result(handle)
-            metadata = backend.get_metadata(handle)
-            print([qm.physical_name for qm in metadata.request.qubit_mapping])
-
-        :param handle: handle to results
-        :type handle: ResultHandle
-        :return: Metadata corresponding to handle
-        :rtype: Metadata
-        """
-        self._check_handle_type(handle)
-        if handle in self._cache and "metadata" in self._cache[handle]:
-            return cast(Metadata, self._cache[handle]["metadata"])
-        # Wait for job to finish, capture metadata and store it in cache
-        timeout = kwargs.get("timeout", 900)
-        run_id = UUID(bytes=cast(bytes, handle[0]))
-        run_result = self._client.wait_for_results(
-            run_id, timeout_secs=cast(float, timeout)
-        )
-        self._cache[handle]["metadata"] = run_result.metadata
-        return cast(Metadata, self._cache[handle]["metadata"])
-
-
-def _as_node(qname: str) -> Node:
-    assert qname.startswith("QB")
-    x = int(qname[2:])
-    assert x >= 1
-    return Node(x - 1)
-
-
-def _as_name(qnode: Node) -> str:
-    assert qnode.reg_name == "node"
-    return f"QB{qnode.index[0] + 1}"
-
-
-def _translate_iqm(circ: Circuit) -> Tuple[Instruction, ...]:
-    """Convert a circuit in the IQM gate set to IQM list representation."""
-    instrs = []
-    for cmd in circ.get_commands():
-        op = cmd.op
-        qbs = cmd.qubits
-        cbs = cmd.bits
-        optype = op.type
-        params = op.params
-        if optype == OpType.PhasedX:
-            instr = Instruction(
-                name="phased_rx",
-                implementation=None,
-                qubits=(str(qbs[0]),),
-                args={"angle_t": 0.5 * params[0], "phase_t": 0.5 * params[1]},
-            )
-        elif optype == OpType.CZ:
-            instr = Instruction(
-                name="cz",
-                implementation=None,
-                qubits=(str(qbs[0]), str(qbs[1])),
-                args={},
-            )
-        else:
-            assert optype == OpType.Measure
-            instr = Instruction(
-                name="measurement",
-                implementation=None,
-                qubits=(str(qbs[0]),),
-                args={"key": str(cbs[0])},
-            )
-        instrs.append(instr)
-    return tuple(instrs)
-
-
-def _iqm_rebase() -> BasePass:
-    # CX replacement
-    c_cx = Circuit(2)
-    c_cx.add_gate(OpType.PhasedX, [-0.5, 0.5], [1])
-    c_cx.CZ(0, 1)
-    c_cx.add_gate(OpType.PhasedX, [0.5, 0.5], [1])
-
-    # TK1 replacement
-    c_tk1 = (
-        lambda a, b, c: Circuit(1)
-        .add_gate(OpType.PhasedX, [-1, (a - c) / 2], [0])
-        .add_gate(OpType.PhasedX, [1 + b, a], [0])
-    )
-
-    return RebaseCustom({OpType.CZ, OpType.PhasedX}, c_cx, c_tk1)
-
-
-_xcirc = Circuit(1).add_gate(OpType.PhasedX, [1, 0], [0]).add_phase(0.5)
+# Copyright 2020-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import json
+import os
+from typing import cast, Dict, List, Optional, Sequence, Tuple, Union
+from uuid import UUID
+from iqm.iqm_client.iqm_client import Circuit as IQMCircuit
+from iqm.iqm_client.iqm_client import Instruction, IQMClient, Metadata, Status
+import numpy as np
+from pytket.backends import Backend, CircuitStatus, ResultHandle, StatusEnum
+from pytket.backends.backend import KwargTypes
+from pytket.backends.backend_exceptions import CircuitNotRunError
+from pytket.backends.backendinfo import BackendInfo
+from pytket.backends.backendresult import BackendResult
+from pytket.backends.resulthandle import _ResultIdTuple
+from pytket.circuit import Circuit, Node, OpType
+from pytket.extensions.iqm._metadata import __extension_version__
+from pytket.passes import (
+    BasePass,
+    SequencePass,
+    SynthesiseTket,
+    FullPeepholeOptimise,
+    FlattenRegisters,
+    RebaseCustom,
+    DecomposeBoxes,
+    RemoveRedundancies,
+    DefaultMappingPass,
+    DelayMeasures,
+    SimplifyInitial,
+)
+from pytket.predicates import (
+    ConnectivityPredicate,
+    GateSetPredicate,
+    NoClassicalControlPredicate,
+    NoFastFeedforwardPredicate,
+    NoBarriersPredicate,
+    NoMidMeasurePredicate,
+    NoSymbolsPredicate,
+    Predicate,
+)
+from pytket.architecture import Architecture
+from pytket.utils import prepare_circuit
+from pytket.utils.outcomearray import OutcomeArray
+from .config import IQMConfig
+
+# Mapping of natively supported instructions' names to members of Pytket OpType
+_IQM_PYTKET_OP_MAP = {
+    "phased_rx": OpType.PhasedX,
+    "cz": OpType.CZ,
+    "measurement": OpType.Measure,
+    "barrier": OpType.Barrier,
+}
+
+
+class IqmAuthenticationError(Exception):
+    """Raised when there is no IQM access credentials available."""
+
+    def __init__(self) -> None:
+        super().__init__("No IQM access credentials provided or found in config file.")
+
+
+class IQMBackend(Backend):
+    """
+    Interface to an IQM device or simulator.
+    """
+
+    _supports_shots = True
+    _supports_counts = True
+    _supports_contextual_optimisation = True
+    _persistent_handles = True
+
+    def __init__(
+        self,
+        url: str,
+        arch: Optional[List[List[str]]] = None,
+        auth_server_url: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+    ):
+        """
+        Construct a new IQM backend.
+
+        Requires _either_ a valid auth server URL, username and password, _or_ a tokens
+        file.
+
+        Auth server URL, username and password can either be provided as parameters or
+        set in config using :py:meth:`pytket.extensions.iqm.set_iqm_config`.
+
+        Path to the tokens file is read from the environmment variable
+        ``IQM_TOKENS_FILE``. If set, this overrides any other credentials provided as
+        arguments.
+
+        :param url: base URL for requests
+        :param arch: Optional list of couplings between the qubits defined, if
+        not set the default value from the server is used.
+        :param auth_server_url: base URL of authentication server
+        :param username: IQM username
+        :param password: IQM password
+        """
+        super().__init__()
+        self._url = url
+        config = IQMConfig.from_default_config_file()
+
+        if auth_server_url is None:
+            auth_server_url = config.auth_server_url
+        tokens_file = os.getenv("IQM_TOKENS_FILE")
+        if username is None:
+            username = config.username
+        if password is None:
+            password = config.password
+        if (username is None or password is None) and tokens_file is None:
+            raise IqmAuthenticationError()
+
+        if tokens_file is None:
+            self._client = IQMClient(
+                self._url,
+                auth_server_url=auth_server_url,
+                username=username,
+                password=password,
+            )
+        else:
+            self._client = IQMClient(self._url, tokens_file=tokens_file)
+        _iqmqa = self._client.get_quantum_architecture()
+        self._operations = [_IQM_PYTKET_OP_MAP[op] for op in _iqmqa.operations]
+        self._qubits = [_as_node(qb) for qb in _iqmqa.qubits]
+        self._n_qubits = len(self._qubits)
+        if arch is None:
+            arch = _iqmqa.qubit_connectivity
+        coupling = [(_as_node(a), _as_node(b)) for (a, b) in arch]
+        if any(qb not in self._qubits for couple in coupling for qb in couple):
+            raise ValueError("Architecture contains qubits not in device")
+        self._arch = Architecture(coupling)
+        self._backendinfo = BackendInfo(
+            name=type(self).__name__,
+            device_name=_iqmqa.name,
+            version=__extension_version__,
+            architecture=self._arch,
+            gate_set=set(self._operations),
+        )
+
+    @property
+    def backend_info(self) -> BackendInfo:
+        return self._backendinfo
+
+    @property
+    def required_predicates(self) -> List[Predicate]:
+        return [
+            NoClassicalControlPredicate(),
+            NoFastFeedforwardPredicate(),
+            NoBarriersPredicate(),
+            NoMidMeasurePredicate(),
+            NoSymbolsPredicate(),
+            GateSetPredicate(set(self._operations)),
+            ConnectivityPredicate(self._arch),
+        ]
+
+    def rebase_pass(self) -> BasePass:
+        return _iqm_rebase()
+
+    def default_compilation_pass(self, optimisation_level: int = 1) -> BasePass:
+        assert optimisation_level in range(3)
+        passes = [DecomposeBoxes(), FlattenRegisters()]
+        if optimisation_level == 0:
+            passes.append(self.rebase_pass())  # to satisfy MaxTwoQubitGatesPredicate
+        elif optimisation_level == 1:
+            passes.append(SynthesiseTket())
+        elif optimisation_level == 2:
+            passes.append(FullPeepholeOptimise())
+        passes.append(DefaultMappingPass(self._arch))
+        passes.append(DelayMeasures())
+        passes.append(self.rebase_pass())
+        passes.append(RemoveRedundancies())
+        return SequencePass(passes)
+
+    @property
+    def _result_id_type(self) -> _ResultIdTuple:
+        return (bytes, str)
+
+    def process_circuits(
+        self,
+        circuits: Sequence[Circuit],
+        n_shots: Union[None, int, Sequence[Optional[int]]] = None,
+        valid_check: bool = True,
+        **kwargs: KwargTypes,
+    ) -> List[ResultHandle]:
+        """
+        See :py:meth:`pytket.backends.Backend.process_circuits`.
+
+        Supported `kwargs`:
+        - `postprocess`: apply end-of-circuit simplifications and classical
+          postprocessing to improve fidelity of results (bool, default False)
+        - `simplify_initial`: apply the pytket ``SimplifyInitial`` pass to improve
+          fidelity of results assuming all qubits initialized to zero (bool, default
+          False)
+        """
+        circuits = list(circuits)
+        n_shots_list = Backend._get_n_shots_as_list(
+            n_shots,
+            len(circuits),
+            optional=False,
+        )
+
+        if valid_check:
+            self._check_all_circuits(circuits)
+
+        postprocess = kwargs.get("postprocess", False)
+        simplify_initial = kwargs.get("postprocess", False)
+
+        handles = []
+        for i, (c, n_shots) in enumerate(zip(circuits, n_shots_list)):
+            if postprocess:
+                c0, ppcirc = prepare_circuit(c, allow_classical=False, xcirc=_xcirc)
+                ppcirc_rep = ppcirc.to_dict()
+            else:
+                c0, ppcirc_rep = c, None
+            if simplify_initial:
+                SimplifyInitial(
+                    allow_classical=False, create_all_qubits=True, xcirc=_xcirc
+                ).apply(c0)
+            instrs = _translate_iqm(c0)
+            qm = {str(qb): _as_name(cast(Node, qb)) for qb in c.qubits}
+            iqmc = IQMCircuit(
+                name=c.name if c.name else f"circuit_{i}",
+                instructions=instrs,
+                metadata=None,
+            )
+            run_id = self._client.submit_circuits(
+                [iqmc], qubit_mapping=qm, shots=n_shots
+            )
+            handles.append(ResultHandle(run_id.bytes, json.dumps(ppcirc_rep)))
+        for handle in handles:
+            self._cache[handle] = dict()
+        return handles
+
+    def _update_cache_result(
+        self, handle: ResultHandle, result_dict: Dict[str, BackendResult]
+    ) -> None:
+        if handle in self._cache:
+            self._cache[handle].update(result_dict)
+        else:
+            self._cache[handle] = result_dict
+
+    def circuit_status(self, handle: ResultHandle) -> CircuitStatus:
+        self._check_handle_type(handle)
+        run_id = UUID(bytes=cast(bytes, handle[0]))
+        run_result = self._client.get_run(run_id)
+        status = run_result.status
+        if status == Status.PENDING_EXECUTION:
+            return CircuitStatus(StatusEnum.SUBMITTED)
+        elif status == Status.READY:
+            measurements = cast(dict, run_result.measurements)[0]
+            shots = OutcomeArray.from_readouts(
+                np.array(
+                    [[r[0] for r in rlist] for cbstr, rlist in measurements.items()],
+                    dtype=int,
+                )
+                .transpose()
+                .tolist()
+            )
+            ppcirc_rep = json.loads(cast(str, handle[1]))
+            ppcirc = Circuit.from_dict(ppcirc_rep) if ppcirc_rep is not None else None
+            self._update_cache_result(
+                handle, {"result": BackendResult(shots=shots, ppcirc=ppcirc)}
+            )
+            return CircuitStatus(StatusEnum.COMPLETED)
+        else:
+            assert status == Status.FAILED
+            return CircuitStatus(StatusEnum.ERROR, cast(str, run_result.message))
+
+    def get_result(self, handle: ResultHandle, **kwargs: KwargTypes) -> BackendResult:
+        """
+        See :py:meth:`pytket.backends.Backend.get_result`.
+        Supported kwargs: `timeout` (default 900).
+        """
+        try:
+            return super().get_result(handle)
+        except CircuitNotRunError:
+            timeout = kwargs.get("timeout", 900)
+            # Wait for job to finish; result will then be in the cache.
+            run_id = UUID(bytes=cast(bytes, handle[0]))
+            self._client.wait_for_results(run_id, timeout_secs=cast(float, timeout))
+            circuit_status = self.circuit_status(handle)
+            if circuit_status.status is StatusEnum.COMPLETED:
+                return cast(BackendResult, self._cache[handle]["result"])
+            else:
+                assert circuit_status.status is StatusEnum.ERROR
+                raise RuntimeError(circuit_status.message)
+
+    def get_metadata(self, handle: ResultHandle, **kwargs: KwargTypes) -> Metadata:
+        """Return the metadata corresponding to the handle.
+
+        Use keyword arguments to specify parameters to be used in retrieving
+        the metadata.
+
+        * `timeout`: maximum time to wait for remote job to finish
+
+        Example usage:
+            n_shots = 100
+            backend.run_circuit(circuit, n_shots=n_shots, timeout=30)
+            handle = backend.process_circuits([circuit], n_shots=n_shots)[0]
+            result = backend.get_result(handle)
+            metadata = backend.get_metadata(handle)
+            print([qm.physical_name for qm in metadata.request.qubit_mapping])
+
+        :param handle: handle to results
+        :type handle: ResultHandle
+        :return: Metadata corresponding to handle
+        :rtype: Metadata
+        """
+        self._check_handle_type(handle)
+        if handle in self._cache and "metadata" in self._cache[handle]:
+            return cast(Metadata, self._cache[handle]["metadata"])
+        # Wait for job to finish, capture metadata and store it in cache
+        timeout = kwargs.get("timeout", 900)
+        run_id = UUID(bytes=cast(bytes, handle[0]))
+        run_result = self._client.wait_for_results(
+            run_id, timeout_secs=cast(float, timeout)
+        )
+        self._cache[handle]["metadata"] = run_result.metadata
+        return cast(Metadata, self._cache[handle]["metadata"])
+
+
+def _as_node(qname: str) -> Node:
+    assert qname.startswith("QB")
+    x = int(qname[2:])
+    assert x >= 1
+    return Node(x - 1)
+
+
+def _as_name(qnode: Node) -> str:
+    assert qnode.reg_name == "node"
+    return f"QB{qnode.index[0] + 1}"
+
+
+def _translate_iqm(circ: Circuit) -> Tuple[Instruction, ...]:
+    """Convert a circuit in the IQM gate set to IQM list representation."""
+    instrs = []
+    for cmd in circ.get_commands():
+        op = cmd.op
+        qbs = cmd.qubits
+        cbs = cmd.bits
+        optype = op.type
+        params = op.params
+        if optype == OpType.PhasedX:
+            instr = Instruction(
+                name="phased_rx",
+                implementation=None,
+                qubits=(str(qbs[0]),),
+                args={"angle_t": 0.5 * params[0], "phase_t": 0.5 * params[1]},
+            )
+        elif optype == OpType.CZ:
+            instr = Instruction(
+                name="cz",
+                implementation=None,
+                qubits=(str(qbs[0]), str(qbs[1])),
+                args={},
+            )
+        else:
+            assert optype == OpType.Measure
+            instr = Instruction(
+                name="measurement",
+                implementation=None,
+                qubits=(str(qbs[0]),),
+                args={"key": str(cbs[0])},
+            )
+        instrs.append(instr)
+    return tuple(instrs)
+
+
+def _iqm_rebase() -> BasePass:
+    # CX replacement
+    c_cx = Circuit(2)
+    c_cx.add_gate(OpType.PhasedX, [-0.5, 0.5], [1])
+    c_cx.CZ(0, 1)
+    c_cx.add_gate(OpType.PhasedX, [0.5, 0.5], [1])
+
+    # TK1 replacement
+    c_tk1 = (
+        lambda a, b, c: Circuit(1)
+        .add_gate(OpType.PhasedX, [-1, (a - c) / 2], [0])
+        .add_gate(OpType.PhasedX, [1 + b, a], [0])
+    )
+
+    return RebaseCustom({OpType.CZ, OpType.PhasedX}, c_cx, c_tk1)
+
+
+_xcirc = Circuit(1).add_gate(OpType.PhasedX, [1, 0], [0]).add_phase(0.5)
```

## Comparing `pytket_iqm-0.8.0.dist-info/LICENSE` & `pytket_iqm-0.9.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `pytket_iqm-0.8.0.dist-info/METADATA` & `pytket_iqm-0.9.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-Metadata-Version: 2.1
-Name: pytket-iqm
-Version: 0.8.0
-Summary: Extension for pytket, providing access to IQM backends
-Author: TKET development team
-Author-email: tket-support@cambridgequantum.com
-License: Apache 2
-Project-URL: Documentation, https://cqcl.github.io/pytket-iqm/api/index.html
-Project-URL: Source, https://github.com/CQCL/pytket-iqm
-Project-URL: Tracker, https://github.com/CQCL/pytket-iqm/issues
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pytket ~=1.21
-Requires-Dist: iqm-client ~=14.0
-
-# pytket-iqm
-
-[Pytket](https://cqcl.github.io/tket/pytket/api/index.html) is a python module
-providing an extensive set of tools for compiling and executing quantum circuits.
-
-`pytket-iqm` is an extension to `pytket` that allows `pytket` circuits to be
-executed on [IQM](https://meetiqm.com/)'s quantum devices and simulators.
-
-## Getting started
-
-`pytket-iqm` is available for Python 3.8, 3.9 and 3.10, on Linux, macOS
-and Windows. To install, run:
-
-```shell
-pip install pytket-iqm
-```
-
-This will install `pytket` if it isn't already installed, and add new classes
-and methods into the `pytket.extensions` namespace.
-
-API documentation is available
-[here](https://cqcl.github.io/pytket-iqm/api/index.html).
-
-Under the hood, `pytket-iqm` uses `iqm-client` to interact with the devices. See
-the IQM Client [documentation](https://iqm-finland.github.io/iqm-client/) and
-Pytket [documentation](https://cqcl.github.io/tket/pytket/api/) for more info.
-
-To use the integration, initialise an `IQMBackend`, construct a Pytket circuit,
-compile it and run. Here is a small example of running a GHZ state circuit:
-
-```python
-from pytket.extensions.iqm import IQMBackend
-from pytket.circuit import Circuit
-
-backend = IQMBackend(
-	url="https://demo.qc.iqm.fi/cocos",
-	auth_server_url="https://demo.qc.iqm.fi/auth",
-	username="USERNAME",
-	password="PASSWORD",
-)
-
-circuit = Circuit(3, 3)
-circuit.H(0)
-circuit.CX(0, 1)
-circuit.CX(0, 2)
-circuit.measure_all()
-compiled_circuit = backend.get_compiled_circuit(circuit)
-
-result = backend.run_circuit(compiled_circuit, n_shots=100)
-print(result.get_shots())
-```
-
-The IQM Client documentation includes the [set of currently supported
-instructions]
-(https://iqm-finland.github.io/iqm-client/api/iqm_client.iqm_client.html).
-`pytket-iqm` retrieves the set from the IQM backend during the initialisation;
-then `get_compiled_circuit()` takes care of compiling the circuit into the
-form suitable to run on the backend.
-
-During the backend initialisation, `pytket-iqm` also retrieves the names of
-physical qubits and qubit connectivity. You can override the qubit connectivity
-by providing the `arch` parameter to the `IQMBackend` constructor, but it generally
-does not make sense, since the IQM server reports the valid quantum architecture
-relevant to the given backend URL.
-
-(Note: At the moment IQM does not provide a quantum computing service open to the 
-general public. Please contact our [sales team](https://www.meetiqm.com/contact/) 
-to set up your access to an IQM quantum computer.)
-
-## Bugs and feature requests
-
-Please file bugs and feature requests on the GitHub
-[issue tracker](https://github.com/CQCL/pytket-iqm/issues).
-
-## Development
-
-To install an extension in editable mode, simply change to its subdirectory
-within the `modules` directory, and run:
-
-```shell
-pip install -e .
-```
-
-## Contributing
-
-Pull requests are welcome. To make a PR, first fork the repo, make your proposed
-changes on the `develop` branch, and open a PR from your fork. If it passes
-tests and is accepted after review, it will be merged in.
-
-### Code style
-
-#### Formatting
-
-All code should be formatted using
-[black](https://black.readthedocs.io/en/stable/), with default options. This is
-checked on the CI.
-
-#### Type annotation
-
-On the CI, [mypy](https://mypy.readthedocs.io/en/stable/) is used as a static
-type checker and all submissions must pass its checks. You should therefore run
-`mypy` locally on any changed files before submitting a PR. Because of the way
-extension modules embed themselves into the `pytket` namespace this is a little
-complicated, but it should be sufficient to run the script `modules/mypy-check`
-(passing as a single argument the root directory of the module to test). The
-script requires `mypy` 0.800 or above.
-
-#### Linting
-
-We use [pylint](https://pypi.org/project/pylint/) on the CI to check compliance
-with a set of style requirements (listed in `.pylintrc`). You should run
-`pylint` over any changed files before submitting a PR, to catch any issues.
-
-### Tests
-
-To run the tests:
-
-```shell
-cd tests
-pip install -r test-requirements.txt
-pytest
-```
-
-By default, the remote tests, which run against the real backend server, are 
-skipped. To enable them, set the following environment variables:
-
-```shell
-export PYTKET_RUN_REMOTE_TESTS=1
-export PYTKET_REMOTE_IQM_AUTH_SERVER_URL=https://demo.qc.iqm.fi/auth
-export PYTKET_REMOTE_IQM_USERNAME=YOUR_USERNAME
-export PYTKET_REMOTE_IQM_PASSWORD=YOUR_PASSWORD
-```
-
-When adding a new feature, please add a test for it. When fixing a bug, please
-add a test that demonstrates the fix.
+Metadata-Version: 2.1
+Name: pytket-iqm
+Version: 0.9.0
+Summary: Extension for pytket, providing access to IQM backends
+Author: TKET development team
+Author-email: tket-support@cambridgequantum.com
+License: Apache 2
+Project-URL: Documentation, https://tket.quantinuum.com/extensions/pytket-iqm/api/index.html
+Project-URL: Source, https://github.com/CQCL/pytket-iqm
+Project-URL: Tracker, https://github.com/CQCL/pytket-iqm/issues
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pytket ~=1.22
+Requires-Dist: iqm-client ~=14.0
+
+# pytket-iqm
+
+[Pytket](https://tket.quantinuum.com/api-docs/index.html) is a python module
+providing an extensive set of tools for compiling and executing quantum circuits.
+
+`pytket-iqm` is an extension to `pytket` that allows `pytket` circuits to be
+executed on [IQM](https://meetiqm.com/)'s quantum devices and simulators.
+
+## Getting started
+
+`pytket-iqm` is available for Python 3.8, 3.9 and 3.10, on Linux, macOS
+and Windows. To install, run:
+
+```shell
+pip install pytket-iqm
+```
+
+This will install `pytket` if it isn't already installed, and add new classes
+and methods into the `pytket.extensions` namespace.
+
+API documentation is available
+[here](https://tket.quantinuum.com/extensions/pytket-iqm/).
+
+Under the hood, `pytket-iqm` uses `iqm-client` to interact with the devices. See
+the IQM Client [documentation](https://iqm-finland.github.io/iqm-client/) and
+Pytket [documentation](https://tket.quantinuum.com/api-docs/) for more info.
+
+To use the integration, initialise an `IQMBackend`, construct a Pytket circuit,
+compile it and run. Here is a small example of running a GHZ state circuit:
+
+```python
+from pytket.extensions.iqm import IQMBackend
+from pytket.circuit import Circuit
+
+backend = IQMBackend(
+	url="https://demo.qc.iqm.fi/cocos",
+	auth_server_url="https://demo.qc.iqm.fi/auth",
+	username="USERNAME",
+	password="PASSWORD",
+)
+
+circuit = Circuit(3, 3)
+circuit.H(0)
+circuit.CX(0, 1)
+circuit.CX(0, 2)
+circuit.measure_all()
+compiled_circuit = backend.get_compiled_circuit(circuit)
+
+result = backend.run_circuit(compiled_circuit, n_shots=100)
+print(result.get_shots())
+```
+
+The IQM Client documentation includes the [set of currently supported
+instructions]
+(https://iqm-finland.github.io/iqm-client/api/iqm_client.iqm_client.html).
+`pytket-iqm` retrieves the set from the IQM backend during the initialisation;
+then `get_compiled_circuit()` takes care of compiling the circuit into the
+form suitable to run on the backend.
+
+During the backend initialisation, `pytket-iqm` also retrieves the names of
+physical qubits and qubit connectivity. You can override the qubit connectivity
+by providing the `arch` parameter to the `IQMBackend` constructor, but it generally
+does not make sense, since the IQM server reports the valid quantum architecture
+relevant to the given backend URL.
+
+(Note: At the moment IQM does not provide a quantum computing service open to the 
+general public. Please contact our [sales team](https://www.meetiqm.com/contact/) 
+to set up your access to an IQM quantum computer.)
+
+## Bugs and feature requests
+
+Please file bugs and feature requests on the GitHub
+[issue tracker](https://github.com/CQCL/pytket-iqm/issues).
+
+## Development
+
+To install an extension in editable mode, simply change to its subdirectory
+within the `modules` directory, and run:
+
+```shell
+pip install -e .
+```
+
+## Contributing
+
+Pull requests are welcome. To make a PR, first fork the repo, make your proposed
+changes on the `develop` branch, and open a PR from your fork. If it passes
+tests and is accepted after review, it will be merged in.
+
+### Code style
+
+#### Formatting
+
+All code should be formatted using
+[black](https://black.readthedocs.io/en/stable/), with default options. This is
+checked on the CI.
+
+#### Type annotation
+
+On the CI, [mypy](https://mypy.readthedocs.io/en/stable/) is used as a static
+type checker and all submissions must pass its checks. You should therefore run
+`mypy` locally on any changed files before submitting a PR. Because of the way
+extension modules embed themselves into the `pytket` namespace this is a little
+complicated, but it should be sufficient to run the script `modules/mypy-check`
+(passing as a single argument the root directory of the module to test). The
+script requires `mypy` 0.800 or above.
+
+#### Linting
+
+We use [pylint](https://pypi.org/project/pylint/) on the CI to check compliance
+with a set of style requirements (listed in `.pylintrc`). You should run
+`pylint` over any changed files before submitting a PR, to catch any issues.
+
+### Tests
+
+To run the tests:
+
+```shell
+cd tests
+pip install -r test-requirements.txt
+pytest
+```
+
+By default, the remote tests, which run against the real backend server, are 
+skipped. To enable them, set the following environment variables:
+
+```shell
+export PYTKET_RUN_REMOTE_TESTS=1
+export PYTKET_REMOTE_IQM_AUTH_SERVER_URL=https://demo.qc.iqm.fi/auth
+export PYTKET_REMOTE_IQM_USERNAME=YOUR_USERNAME
+export PYTKET_REMOTE_IQM_PASSWORD=YOUR_PASSWORD
+```
+
+When adding a new feature, please add a test for it. When fixing a bug, please
+add a test that demonstrates the fix.
```

## Comparing `pytket_iqm-0.8.0.dist-info/RECORD` & `pytket_iqm-0.9.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pytket/extensions/iqm/__init__.py,sha256=difGgTZ_tiM6MRc2u7TgtOcJ-CYrDKdldGFb4ul38Mg,895
-pytket/extensions/iqm/_metadata.py,sha256=WBvr_B-yy7Rv7vdgZzOpF-0i58iBnQNQS7FwYhrmyzM,68
+pytket/extensions/iqm/__init__.py,sha256=DJB70XQ4qHiGqOMhCCLd4yKT9kBf5cjs0EZLkbvKq5U,874
+pytket/extensions/iqm/_metadata.py,sha256=_h8Dd1vCnIgUFjuM325R4LqKMX0v-8acBN1CxKuo3xs,66
 pytket/extensions/iqm/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pytket/extensions/iqm/backends/__init__.py,sha256=VCV-7IHpWD9GpFOGW656GcpHmcGc8Yck_hYoXhDksI4,708
-pytket/extensions/iqm/backends/config.py,sha256=lUQ2fYsnaBS8sdqx3uYxf0qn3D0ejGxCmzU27U2Z9Zs,1808
-pytket/extensions/iqm/backends/iqm.py,sha256=9Ib31ptu_J8ZAfBMXHvMblsshHxj_R1lHcykWIk-v1M,14948
-pytket_iqm-0.8.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-pytket_iqm-0.8.0.dist-info/METADATA,sha256=-Nr2kEh9D4YYL90-cpHHQp22qPUPFOjpnMAnOv2NK5c,5837
-pytket_iqm-0.8.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-pytket_iqm-0.8.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_iqm-0.8.0.dist-info/RECORD,,
+pytket/extensions/iqm/backends/__init__.py,sha256=jvPqNYcWw-bTjzfLoJ7Q6-0b_cr3H7HDrZeARazG8Gg,690
+pytket/extensions/iqm/backends/config.py,sha256=X-sPH-l9OCw_O8lsW-v8UHJi5q_xLHIAxeN7qwqphHY,1752
+pytket/extensions/iqm/backends/iqm.py,sha256=4GS5h-Ll5Neg1gmUc1pzEQFoWKvytMpIspTlc-AhtyA,14549
+pytket_iqm-0.9.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_iqm-0.9.0.dist-info/METADATA,sha256=ryjIHM4wYGG2CrAIQsfl-TTfSnXzJfHq3NWPJXGiiNw,5689
+pytket_iqm-0.9.0.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+pytket_iqm-0.9.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_iqm-0.9.0.dist-info/RECORD,,
```

