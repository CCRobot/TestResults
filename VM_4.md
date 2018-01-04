```
Executed on w1604chak000000
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0100 9180k  100 9180k    0     0  10.1M      0 --:--:-- --:--:-- --:--:-- 10.1M
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9  121M    9 11.0M    0     0  10.0M      0  0:00:12  0:00:01  0:00:11 10.0M 24  121M   24 29.5M    0     0  14.1M      0  0:00:08  0:00:02  0:00:06 14.1M 39  121M   39 47.6M    0     0  15.4M      0  0:00:07  0:00:03  0:00:04 15.4M 52  121M   52 63.7M    0     0  15.6M      0  0:00:07  0:00:04  0:00:03 15.6M 65  121M   65 80.0M    0     0  15.6M      0  0:00:07  0:00:05  0:00:02 15.9M 80  121M   80 98.0M    0     0  16.0M      0  0:00:07  0:00:06  0:00:01 17.3M 95  121M   95  116M    0     0  16.4M      0  0:00:07  0:00:07 --:--:-- 17.4M100  121M  100  121M    0     0  16.5M      0  0:00:07  0:00:07 --:--:-- 17.4M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   a13c30b..86f0d57  master     -> origin/master
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
] Testing  RL18_DBG_ubuntu
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```