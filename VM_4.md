```
Executed on ddchakra005.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0 21 11.1M   21 2431k    0     0  3137k      0  0:00:03 --:--:--  0:00:03 3137k100 11.1M  100 11.1M    0     0  7283k      0  0:00:01  0:00:01 --:--:-- 7286k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  6  121M    6 7968k    0     0  7013k      0  0:00:17  0:00:01  0:00:16 7007k 12  121M   12 15.3M    0     0  7376k      0  0:00:16  0:00:02  0:00:14 7374k 20  121M   20 25.4M    0     0  8294k      0  0:00:15  0:00:03  0:00:12 8293k 29  121M   29 35.8M    0     0  8876k      0  0:00:14  0:00:04  0:00:10 8876k 38  121M   38 46.8M    0     0  9339k      0  0:00:13  0:00:05  0:00:08 9744k 45  121M   45 55.8M    0     0  9322k      0  0:00:13  0:00:06  0:00:07 9845k 49  121M   49 60.5M    0     0  8686k      0  0:00:14  0:00:07  0:00:07 9245k 56  121M   56 68.7M    0     0  8659k      0  0:00:14  0:00:08  0:00:06 8888k 63  121M   63 77.9M    0     0  8737k      0  0:00:14  0:00:09  0:00:05 8624k 71  121M   71 87.0M    0     0  8797k      0  0:00:14  0:00:10  0:00:04 8240k 80  121M   80 98.0M    0     0  9015k      0  0:00:13  0:00:11  0:00:02 8641k 88  121M   88  107M    0     0  9092k      0  0:00:13  0:00:12  0:00:01 9670k 95  121M   95  116M    0     0  9088k      0  0:00:13  0:00:13 --:--:-- 9784k100  121M  100  121M    0     0  9042k      0  0:00:13  0:00:13 --:--:-- 9639k
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
] Testing  RL18_DBG_osx
] Connected
done!
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```