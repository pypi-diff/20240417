# Comparing `tmp/gkbus-0.1.81-py3-none-any.whl.zip` & `tmp/gkbus-0.1.82-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 23414 bytes, number of entries: 19
+Zip file size: 23487 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx      539 b- defN 23-Dec-21 00:36 gkbus/__init__.py
 -rw-rw-r--  2.0 unx       48 b- defN 23-Dec-17 17:14 gkbus/exceptions.py
--rw-rw-r--  2.0 unx     1146 b- defN 24-Mar-06 15:03 gkbus/interface/CanInterface.py
--rw-rw-r--  2.0 unx     3207 b- defN 24-Mar-06 15:03 gkbus/interface/Interface.py
--rw-rw-r--  2.0 unx     3246 b- defN 24-Mar-06 15:03 gkbus/interface/KLineInterface.py
+-rw-rw-r--  2.0 unx     1170 b- defN 24-Apr-17 15:13 gkbus/interface/CanInterface.py
+-rw-rw-r--  2.0 unx     3231 b- defN 24-Apr-17 15:14 gkbus/interface/Interface.py
+-rw-rw-r--  2.0 unx     3270 b- defN 24-Apr-17 15:14 gkbus/interface/KLineInterface.py
 -rw-rw-r--  2.0 unx       81 b- defN 23-Dec-10 15:49 gkbus/interface/__init__.py
 -rw-rw-r--  2.0 unx     2264 b- defN 24-Mar-06 15:03 gkbus/interface/kline/KLineSerial.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Dec-10 15:49 gkbus/interface/kline/__init__.py
--rw-rw-r--  2.0 unx      847 b- defN 24-Mar-11 00:23 gkbus/kwp/KWPCommand.py
+-rw-rw-r--  2.0 unx      872 b- defN 24-Apr-17 15:11 gkbus/kwp/KWPCommand.py
 -rw-rw-r--  2.0 unx     2778 b- defN 23-Dec-20 17:13 gkbus/kwp/KWPNegativeStatus.py
--rw-rw-r--  2.0 unx      281 b- defN 24-Mar-11 00:24 gkbus/kwp/KWPResponse.py
+-rw-rw-r--  2.0 unx      306 b- defN 24-Apr-17 15:12 gkbus/kwp/KWPResponse.py
 -rw-rw-r--  2.0 unx      140 b- defN 24-Mar-11 00:30 gkbus/kwp/__init__.py
--rw-rw-r--  2.0 unx     5831 b- defN 24-Mar-06 15:04 gkbus/kwp/commands.py
+-rw-rw-r--  2.0 unx     5855 b- defN 24-Apr-17 15:13 gkbus/kwp/commands.py
 -rw-rw-r--  2.0 unx      973 b- defN 23-Dec-25 09:58 gkbus/kwp/enums.py
--rw-rw-r--  2.0 unx    35149 b- defN 24-Mar-11 00:31 gkbus-0.1.81.dist-info/LICENSE
--rw-rw-r--  2.0 unx      300 b- defN 24-Mar-11 00:31 gkbus-0.1.81.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-11 00:31 gkbus-0.1.81.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 24-Mar-11 00:31 gkbus-0.1.81.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1527 b- defN 24-Mar-11 00:31 gkbus-0.1.81.dist-info/RECORD
-19 files, 58455 bytes uncompressed, 20918 bytes compressed:  64.2%
+-rw-rw-r--  2.0 unx    35149 b- defN 24-Apr-17 15:15 gkbus-0.1.82.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      300 b- defN 24-Apr-17 15:15 gkbus-0.1.82.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 15:15 gkbus-0.1.82.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-17 15:15 gkbus-0.1.82.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1527 b- defN 24-Apr-17 15:15 gkbus-0.1.82.dist-info/RECORD
+19 files, 58601 bytes uncompressed, 20991 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: gkbus/kwp/commands.py
 Comment: 
 
 Filename: gkbus/kwp/enums.py
 Comment: 
 
-Filename: gkbus-0.1.81.dist-info/LICENSE
+Filename: gkbus-0.1.82.dist-info/LICENSE
 Comment: 
 
-Filename: gkbus-0.1.81.dist-info/METADATA
+Filename: gkbus-0.1.82.dist-info/METADATA
 Comment: 
 
-Filename: gkbus-0.1.81.dist-info/WHEEL
+Filename: gkbus-0.1.82.dist-info/WHEEL
 Comment: 
 
-Filename: gkbus-0.1.81.dist-info/top_level.txt
+Filename: gkbus-0.1.82.dist-info/top_level.txt
 Comment: 
 
-Filename: gkbus-0.1.81.dist-info/RECORD
+Filename: gkbus-0.1.82.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gkbus/interface/CanInterface.py

```diff
@@ -1,7 +1,8 @@
+from typing import List
 from scapy.config import conf
 conf.contribs['CANSocket'] = {'use-python-can': False}
 conf.contribs['ISOTP'] = {'use-can-isotp-kernel-module': True}
 from scapy.contrib.cansocket import *
 from scapy.contrib.isotp import *
 import logging
 from .Interface import InterfaceABC
@@ -9,15 +10,15 @@
 
 class CanInterface(InterfaceABC):
 	socket = False
 
 	def __init__ (self, rx_id: int, tx_id: int, interface: str = 'can0'):
 		self.socket = ISOTPNativeSocket(iface=interface, tx_id=tx_id, rx_id=rx_id, padding=True)
 
-	def _execute_internal (self, payload: list[int]) -> list[int]:
+	def _execute_internal (self, payload: List[int]) -> List[int]:
 		response = self.socket.sr1(ISOTP(bytes(payload)), verbose=False)
 
 		data = list(response.data)
 
 		if (len(data) > 2):
 			if (data[0] == 0x7f and data[2] == 0x78): # request received response pending
 				logger.warning('ECU is busy, request received, response pending.')
```

## gkbus/interface/Interface.py

```diff
@@ -1,11 +1,12 @@
 from abc import ABCMeta
 from ..kwp import KWPCommand, KWPResponse, KWPNegativeStatus, KWPNegativeResponseException
 import threading, time
 from gkbus import GKBusTimeoutException
+from typing import List
 
 class InterfaceABC(metaclass=ABCMeta):
 	def init (self, payload: KWPCommand = None, keepalive_payload: KWPCommand = None, keepalive_timeout: int = None) -> None:
 		"""Make the bus ready for sending and receiving commands"""
 		self._init([payload.get_command()] + payload.get_data())
 		self._execute_lock = threading.Lock()
 
@@ -13,15 +14,15 @@
 			self.keepalive_payload = keepalive_payload
 			self.keepalive_timeout = keepalive_timeout
 			self._keepalive_thread = None 
 			self._last_execution_time = time.time()
 			self._keepalive_event = threading.Event()
 			self.start_keepalive()
 
-	def _init (self, payload: list[int]) -> None:
+	def _init (self, payload: List[int]) -> None:
 		"""Make the bus ready for sending and receiving commands"""
 
 	def execute (self, kwp_command: KWPCommand) -> KWPResponse:
 		"""Send KWPCommand and prepare response"""
 		if (not hasattr(self, '_execute_lock')):
 			self._execute_lock = threading.Lock() # not ideal
```

## gkbus/interface/KLineInterface.py

```diff
@@ -1,7 +1,8 @@
+from typing import List
 import time, logging, struct
 from .Interface import InterfaceABC
 from .kline.KLineSerial import KLineSerial
 from gkbus import GKBusTimeoutException
 
 logger = logging.getLogger(__name__)
 
@@ -28,36 +29,36 @@
 		try:
 			self.fetch_response()
 		except GKBusTimeoutException:
 			logger.warning('ftdi fast init failed!')
 
 		self.set_timeout(5)
 
-	def calculate_checksum (self, payload: list[int]) -> int:
+	def calculate_checksum (self, payload: List[int]) -> int:
 		checksum = 0x0
 		for byte in payload:
 			checksum += byte
 		return checksum & 0xFF
 
-	def build_payload (self, data: list[int]) -> bytearray:
+	def build_payload (self, data: List[int]) -> bytearray:
 		data_length = len(data)
 
 		if (data_length < 127):
 			counter = 0x80 + data_length
 		else:
 			counter = 0x80
 			data = [data_length] + data
 
 		tx_id = struct.pack('>h', self.tx_id)
 
 		payload = [counter, *tx_id] + data
 		payload += [self.calculate_checksum(payload)]
 		return bytes(payload)
 
-	def fetch_response (self, recursion_level: int = 0) -> list[int]:
+	def fetch_response (self, recursion_level: int = 0) -> List[int]:
 		counter = self._read(1)
 
 		rx_id, = struct.unpack('>H', self._read(2))
 
 		if (counter == b'\x80'): # more than 127 bytes incoming, counter overflowed. counter is gonna come after IDs
 			counter, = struct.unpack('>B', self._read(1))
 		else:
@@ -79,15 +80,15 @@
 		if (rx_id != self.rx_id): # we are only doing this now because we needed to clear this message out of the buffer
 			if (recursion_level > 3):
 				self.shutdown()
 			return self.fetch_response(recursion_level=recursion_level+1)
 			
 		return [struct.unpack('>B', status)[0]] + data
 
-	def _execute_internal (self, payload: list[int]) -> list[int]:
+	def _execute_internal (self, payload: List[int]) -> List[int]:
 		self._write(self.build_payload(payload))
 		response = self.fetch_response()
 
 		return response
 
 	def _write (self, message: bytearray) -> None:
 		logger.debug('K-Line sending: {}'.format(' '.join([hex(x) for x in message])))
```

## gkbus/kwp/KWPCommand.py

```diff
@@ -1,18 +1,20 @@
+from typing import List
+
 class KWPCommand:
 	command: int = 0x0
 
-	def __init__ (self, data: list[int]=[]):
-		self.data: list[int] = data
+	def __init__ (self, data: List[int]=[]):
+		self.data: List[int] = data
 
 	def set_data (self, data):
 		self.data = data
 		return self
 
-	def get_data (self) -> list[int]:
+	def get_data (self) -> List[int]:
 		return self.data
 
 	def set_command (self, command: int):
 		self.command = command
 		return self
 
 	def get_command (self) -> int:
@@ -20,14 +22,14 @@
 
 	def __str__ (self) -> str:
 		return '<KWPCommand: {} {}>'.format(hex(self.get_command()), ' '.join([hex(x) for x in self.get_data()]))
 
 class KWPCommandWithSubservices(KWPCommand):
 	def __init__ (self, subservice: int, *kwargs):
 		self.subservice: Enum = subservice
-		self.data: list[int] = [subservice.value]
+		self.data: List[int] = [subservice.value]
 		handler = getattr(self, self.subservices[subservice])
 		handler(*kwargs)
 
-	def set_data (self, data: list[int]):
+	def set_data (self, data: List[int]):
 		self.data = [self.subservice.value] + data
 		return self
```

## gkbus/kwp/KWPResponse.py

```diff
@@ -1,12 +1,14 @@
+from typing import List
+
 class KWPResponse:
-	data: list[int] = False
+	data: List[int] = False
 
-	def set_data (self, data: list[int]):
+	def set_data (self, data: List[int]):
 		self.data = data
 		return self
 
-	def get_data (self) -> list[int]:
+	def get_data (self) -> List[int]:
 		return self.data
 
 	def __str__ (self) -> str:
 		return '<KWPResponse: {}>'.format(' '.join([hex(x) for x in self.get_data()]))
```

## gkbus/kwp/commands.py

```diff
@@ -1,10 +1,11 @@
 import struct
 from .KWPCommand import KWPCommand, KWPCommandWithSubservices
 from .enums import *
+from typing import List
 
 class AccessTimingParameters(KWPCommandWithSubservices): # TimingParameterIdentifier
 	command = 0x83
 	subservices = {
 		TimingParameterIdentifier.READ_LIMITS_OF_POSSIBLE_TIMING_PARAMETERS: 'read_limits_of_possible_timing_parameters',
 		TimingParameterIdentifier.SET_TIMING_PARAMETERS_TO_DEFAULT_VALUES: 'set_timing_parameters_to_default_values',
 		TimingParameterIdentifier.READ_CURRENTLY_ACTIVE_TIMING_PARAMETERS: 'read_currently_active_timing_parameters',
@@ -192,21 +193,21 @@
 
 class WriteDataByIdentifier(KWPCommand):
 	command = 0x2E
 
 class WriteDataByLocalIdentifier(KWPCommand):
 	command = 0x3B
 
-	def __init__ (self, record_local_identifier: int, record_value: list[int]):
+	def __init__ (self, record_local_identifier: int, record_value: List[int]):
 		self.set_data([record_local_identifier] + record_value)
 
 class WriteMemoryByAddress(KWPCommand):
 	command = 0x3D
 
-	def __init__ (self, offset: int, data_to_write: list[int]):
+	def __init__ (self, offset: int, data_to_write: List[int]):
 		size = len(data_to_write)
 
 		address = struct.pack('>L', offset)[1:]
 
 		self.set_data([*address, size] + data_to_write)
 
 class StopCommunication(KWPCommand):
```

## Comparing `gkbus-0.1.81.dist-info/LICENSE` & `gkbus-0.1.82.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gkbus-0.1.81.dist-info/RECORD` & `gkbus-0.1.82.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 gkbus/__init__.py,sha256=YHMxL1t9aAfUJtaRvQPTTbXHGWjyImPKjYLGro8i4sE,539
 gkbus/exceptions.py,sha256=LX2uUV-OR0fbG4bN6UPJj-yb3ZlOvvDGUMCE-2dWq6w,48
-gkbus/interface/CanInterface.py,sha256=Jxj0zrlvwhhuKfCO5Jvlm2g533Bku_5ADHaeiBUXBzw,1146
-gkbus/interface/Interface.py,sha256=2LtEcSzTodv2DDUkQFa9lDbaQ1GamIChkMohAXVhYx0,3207
-gkbus/interface/KLineInterface.py,sha256=ewqdoR0G8vmCRQ3FGS3V2rUBWX8LG9791OZU0pKjXhc,3246
+gkbus/interface/CanInterface.py,sha256=sUDzEs0RtKWD8kIiA6LF8gffgm33mnZYh6S9Hxboy2o,1170
+gkbus/interface/Interface.py,sha256=gJg5aQ4JmpanSWoSqo9jaH051hPWnbb1xzAmVH0VCFY,3231
+gkbus/interface/KLineInterface.py,sha256=5so9uWNIlzBPt6e1cnC927RsjZ3qDq_Yu677adQ48fM,3270
 gkbus/interface/__init__.py,sha256=QqDSXMQeS7ba2P7YaWIVnf2Fz6QBLId2swNTr-Rz0Vo,81
 gkbus/interface/kline/KLineSerial.py,sha256=GicX-x-y3s2drrypc4szBNZuVhC4f1KRZtnVXrMjRo8,2264
 gkbus/interface/kline/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gkbus/kwp/KWPCommand.py,sha256=GQduWdW4xwdWD5VmCd0G8aA3m3qp8wr6yzxzsSFrNbQ,847
+gkbus/kwp/KWPCommand.py,sha256=Ste5Gu9xWfFnA7E4u6QUeIBoBHwuR9O2B8zyWlxjExg,872
 gkbus/kwp/KWPNegativeStatus.py,sha256=HjRXNRENBnuG6geos6VS1R1vDqnx3rA17jowhXsJxS8,2778
-gkbus/kwp/KWPResponse.py,sha256=KTo4EaOJiXXnqA8dEIeofgvrEI_aoavggcGjKWl7vkg,281
+gkbus/kwp/KWPResponse.py,sha256=B_-yDpTG2tEj5XSog0UzFcdZVlDmQVQFVRQiuvp1pXA,306
 gkbus/kwp/__init__.py,sha256=EGU89IHH9_p0F_DCiy464Q5LWDit1ueSZFBY4IQQa5Y,140
-gkbus/kwp/commands.py,sha256=FBAqxuXK-2-ZTuZNH-j1vdzauKzsh0sx3ggHYIXDKhI,5831
+gkbus/kwp/commands.py,sha256=Gb3PIeWrxLJX62Jgjae-4PbSUX3qIB-7ivgSpEoP5aY,5855
 gkbus/kwp/enums.py,sha256=5wP3VlFnbvgJHFA7q0W6pRmJCdZkvHQ2eeeJULdUrYQ,973
-gkbus-0.1.81.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-gkbus-0.1.81.dist-info/METADATA,sha256=mq6tyg8Lwax0EYxFHDoSivLjTBpDsEbpmtafICOdnoM,300
-gkbus-0.1.81.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-gkbus-0.1.81.dist-info/top_level.txt,sha256=SH8xkZKh5XisjZUlhbOEvdOX3kDL5RKX_s_YVTNhzgo,6
-gkbus-0.1.81.dist-info/RECORD,,
+gkbus-0.1.82.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+gkbus-0.1.82.dist-info/METADATA,sha256=fiJfKJjbX_TYft0CBG7lOGOvUrbC5eFuI13PUX8tIyU,300
+gkbus-0.1.82.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+gkbus-0.1.82.dist-info/top_level.txt,sha256=SH8xkZKh5XisjZUlhbOEvdOX3kDL5RKX_s_YVTNhzgo,6
+gkbus-0.1.82.dist-info/RECORD,,
```

