```
Executed on ddchakra003.local
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0 11.1M    0 81499    0     0   247k      0  0:00:45 --:--:--  0:00:45  247k100 11.1M  100 11.1M    0     0  8855k      0  0:00:01  0:00:01 --:--:-- 8857k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  9  129M    9 12.0M    0     0  11.7M      0  0:00:10  0:00:01  0:00:09 11.7M 21  129M   21 28.2M    0     0  13.9M      0  0:00:09  0:00:02  0:00:07 13.9M 33  129M   33 43.0M    0     0  14.2M      0  0:00:09  0:00:03  0:00:06 14.2M 46  129M   46 59.8M    0     0  14.9M      0  0:00:08  0:00:04  0:00:04 14.9M 54  129M   54 70.8M    0     0  14.1M      0  0:00:09  0:00:05  0:00:04 14.1M 64  129M   64 83.7M    0     0  13.9M      0  0:00:09  0:00:06  0:00:03 14.3M 77  129M   77  100M    0     0  14.2M      0  0:00:09  0:00:07  0:00:02 14.3M 89  129M   89  116M    0     0  14.4M      0  0:00:08  0:00:08 --:--:-- 14.5M100  129M  100  129M    0     0  14.5M      0  0:00:08  0:00:08 --:--:-- 14.3M
untar ChakraCore
untar HelixClient
From https://github.com/Microsoft/ChakraCore
   c27adba..79df905  master      -> origin/master
   745ddf8..148c8af  intl-icu    -> origin/intl-icu
   cf780ac..e20d5c6  release/1.7 -> origin/release/1.7
   3e68e46..b5cf4ec  release/1.8 -> origin/release/1.8
Updating c27adba..79df905
Fast-forward
 bin/ChakraCore/ChakraCore.def                      |   2 +
 bin/NativeTests/JsRTApiTest.cpp                    | 211 +++++++++++++++++++++
 bin/ch/ChakraRtInterface.h                         |   5 +-
 lib/Backend/BackwardPass.cpp                       |   8 +-
 lib/Backend/BailOut.cpp                            |   8 +-
 lib/Backend/BailOut.h                              |   5 +-
 lib/Backend/FlowGraph.cpp                          |   3 +
 lib/Backend/GlobOpt.cpp                            |  65 ++++---
 lib/Backend/GlobOpt.h                              |   1 +
 lib/Backend/GlobOptBailOut.cpp                     |  29 +--
 lib/Backend/GlobOptBlockData.cpp                   |  38 +++-
 lib/Backend/GlobOptBlockData.h                     |   1 +
 lib/Backend/IR.cpp                                 |  13 +-
 lib/Backend/IR.h                                   |  20 +-
 lib/Backend/JnHelperMethod.cpp                     |   4 +-
 lib/Backend/amd64/LinearScanMD.cpp                 |   8 +-
 lib/Backend/i386/LinearScanMD.cpp                  |   8 +-
 lib/Common/CommonDefines.h                         |   3 -
 lib/Common/ConfigFlagsList.h                       |   5 -
 lib/Jsrt/ChakraCore.h                              |  47 +++++
 lib/Jsrt/Jsrt.cpp                                  |  76 ++++++--
 lib/Runtime/Base/FunctionBody.cpp                  |   3 +
 lib/Runtime/ByteCode/ByteCodeEmitter.cpp           |  18 +-
 lib/Runtime/ByteCode/ByteCodeGenerator.cpp         |   2 +-
 lib/Runtime/Debug/TTEventLog.cpp                   |   3 +-
 lib/Runtime/Debug/TTRuntmeInfoTracker.cpp          |   1 +
 lib/Runtime/Debug/TTSerializeEnum.h                |   4 +
 lib/Runtime/Debug/TTSnapObjects.cpp                | 189 +++++++++++++++---
 lib/Runtime/Debug/TTSnapObjects.h                  |  37 +++-
 lib/Runtime/Debug/TTSnapshot.cpp                   |  17 +-
 lib/Runtime/Debug/TTSupport.h                      |   2 +
 lib/Runtime/Language/InterpreterStackFrame.cpp     |  19 +-
 lib/Runtime/Language/JavascriptOperators.cpp       |   2 +-
 lib/Runtime/Language/amd64/amd64_Thunks.S          |  78 --------
 lib/Runtime/Library/JavascriptExternalFunction.cpp |  23 ++-
 lib/Runtime/Library/JavascriptExternalFunction.h   |  11 +-
 lib/Runtime/Library/JavascriptGenerator.cpp        |  18 +-
 .../Library/JavascriptGeneratorFunction.cpp        |  62 +++++-
 lib/Runtime/Library/JavascriptGeneratorFunction.h  |   2 +
 lib/Runtime/Library/JavascriptLibrary.cpp          |  10 +-
 lib/Runtime/Library/JavascriptLibrary.h            |   3 +-
 lib/Runtime/Library/JavascriptPromise.cpp          | 113 ++++++++++-
 lib/Runtime/Library/amd64/JavascriptFunctionA.S    |  12 --
 pal/inc/pal.h                                      |   2 +
 pal/src/map/virtual.cpp                            |   7 +-
 pal/src/memory/heap.cpp                            |   8 +-
 test/AsmJs/rlexe.xml                               |  11 +-
 test/Bugs/rlexe.xml                                |   7 +-
 test/Optimizer/capturedValuesBugs.js               |  29 +++
 test/Optimizer/rlexe.xml                           |  12 ++
 test/Optimizer/test146.js                          |  52 +++++
 test/Optimizer/test147.js                          |  19 ++
 test/TTBasic/asyncAwaitBasic.js                    |  75 ++++++++
 test/TTBasic/asyncAwaitBasicRecord.baseline        |   5 +
 test/TTBasic/asyncAwaitBasicReplay_1.baseline      |   7 +
 test/TTBasic/asyncAwaitBasicReplay_2.baseline      |   7 +
 test/TTBasic/asyncAwaitBasicReplay_3.baseline      |   4 +
 test/TTBasic/asyncAwaitBasicReplay_4.baseline      |   4 +
 test/TTBasic/asyncAwaitBasicReplay_5.baseline      |   3 +
 test/TTBasic/rlexe.xml                             |  51 ++++-
 test/es6/bug_OS14562349.js                         |  24 +++
 test/es6/rlexe.xml                                 |   7 +
 test/rlexedirs.xml                                 |   2 +-
 test/wasm/limits.js                                |   2 +-
 test/wasm/rlexe.xml                                |  50 ++---
 test/wasm/signextend.js                            |   4 +-
 tools/compile_clang.sh                             |  34 +++-
 67 files changed, 1280 insertions(+), 335 deletions(-)
 create mode 100644 test/Optimizer/test146.js
 create mode 100644 test/Optimizer/test147.js
 create mode 100644 test/TTBasic/asyncAwaitBasic.js
 create mode 100644 test/TTBasic/asyncAwaitBasicRecord.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_1.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_2.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_3.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_4.baseline
 create mode 100644 test/TTBasic/asyncAwaitBasicReplay_5.baseline
 create mode 100644 test/es6/bug_OS14562349.js
] Connecting to server: {
  "host": "ccrobot.westus2.cloudapp.azure.com:8001",
  "command": "testClient"
}
] Connected
] Request sent successfully
] Testing  DEBUG_osx
] Connected
] Request sent successfully
-e ___ TEST_EXIT_CODE := 0 ___

```