```
Executed on DDCHAKRA002.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 14 11.1M   14 1615k    0     0  3987k      0  0:00:02 --:--:--  0:00:02 3989k100 11.1M  100 11.1M    0     0  9688k      0  0:00:01  0:00:01 --:--:-- 9694k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  7  121M    7 9024k    0     0  7958k      0  0:00:15  0:00:01  0:00:14 7957k 13  121M   13 16.1M    0     0  7777k      0  0:00:16  0:00:02  0:00:14 7774k 19  121M   19 24.0M    0     0  7835k      0  0:00:15  0:00:03  0:00:12 7834k 27  121M   27 33.4M    0     0  8284k      0  0:00:15  0:00:04  0:00:11 8282k 34  121M   34 41.9M    0     0  8357k      0  0:00:14  0:00:05  0:00:09 8714k 42  121M   42 51.7M    0     0  8640k      0  0:00:14  0:00:06  0:00:08 8795k 50  121M   50 61.5M    0     0  8839k      0  0:00:14  0:00:07  0:00:07 9292k 57  121M   57 69.8M    0     0  8798k      0  0:00:14  0:00:08  0:00:06 9401k 65  121M   65 79.2M    0     0  8885k      0  0:00:14  0:00:09  0:00:05 9381k 73  121M   73 90.1M    0     0  9112k      0  0:00:13  0:00:10  0:00:03 9888k 83  121M   83  101M    0     0  9378k      0  0:00:13  0:00:11  0:00:02 10.0M 91  121M   91  111M    0     0  9377k      0  0:00:13  0:00:12  0:00:01  9.9M 97  121M   97  118M    0     0  9103k      0  0:00:13  0:00:13 --:--:-- 9582k100  121M  100  121M    0     0  8964k      0  0:00:13  0:00:13 --:--:-- 9116k
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   a13c30b..86f0d57  master      -> origin/master
   1209352..500baba  release/1.8 -> origin/release/1.8
Updating a13c30b..86f0d57
Fast-forward
 lib/Common/Memory/HeapAllocator.h                  |  53 +++
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp           |  10 +-
 .../Language/JavascriptExceptionOperators.cpp      | 182 +++++----
 .../Language/JavascriptExceptionOperators.h        |   2 +-
 lib/Runtime/Language/JavascriptStackWalker.cpp     |  27 +-
 lib/Runtime/Language/JavascriptStackWalker.h       |   2 +-
 lib/Runtime/Library/WasmLibrary.cpp                |   2 +-
 lib/Runtime/Library/WebAssemblyModule.cpp          |  31 +-
 lib/Runtime/Library/WebAssemblyModule.h            |  13 +-
 lib/WasmReader/Chakra.WasmReader.vcxproj           |   2 +-
 lib/WasmReader/Chakra.WasmReader.vcxproj.filters   |   2 +-
 lib/WasmReader/WasmBinaryOpCodes.h                 | 447 +++++++++++----------
 lib/WasmReader/WasmBinaryOpcodesSimd.h             | 298 +++++++-------
 lib/WasmReader/WasmBinaryReader.cpp                |  43 +-
 lib/WasmReader/WasmBinaryReader.h                  |   3 +-
 lib/WasmReader/WasmByteCodeGenerator.cpp           |  30 +-
 lib/WasmReader/WasmParseTree.h                     |   4 +-
 lib/WasmReader/WasmSignature.cpp                   |  45 ++-
 lib/WasmReader/WasmSignature.h                     |   1 +
 pal/inc/rt/palrt.h                                 |   4 +-
 test/Bugs/bug14323330.js                           |  49 +++
 test/Bugs/rlexe.xml                                |   7 +
 test/es7/arraybuffer_constructor.js                |  33 --
 test/es7/arraybuffer_transfer.js                   |  37 --
 test/es7/rlexe.xml                                 |  23 --
 test/wasm/binary.js                                |   8 +-
 test/wasm/i64.js                                   |   8 +-
 test/wasm/limits.js                                |   4 +-
 test/wasm/nestedblocks.js                          |   4 +-
 test/wasm/regress.js                               | 158 ++++++--
 test/wasm/rlexe.xml                                |  19 +-
 test/wasm/table_signatures.js                      | 118 ++++++
 32 files changed, 970 insertions(+), 699 deletions(-)
 create mode 100644 test/Bugs/bug14323330.js
 delete mode 100644 test/es7/arraybuffer_constructor.js
 delete mode 100644 test/es7/arraybuffer_transfer.js
 create mode 100644 test/wasm/table_signatures.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  RL18_PACK
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```